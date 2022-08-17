
# Notiboy Smart Contract

Smart contract is written [here](sc.py)

Supports:
1. Sending public notification
https://github.com/Notiboy-Project/notiboy-sc/blob/842017f3ca35c390cacc128e98726b6cc8f36410/sc.py#L229
2. Sending personal notification to user
https://github.com/Notiboy-Project/notiboy-sc/blob/842017f3ca35c390cacc128e98726b6cc8f36410/sc.py#L211
3. Watermarking dapps with verified tag
https://github.com/Notiboy-Project/notiboy-sc/blob/842017f3ca35c390cacc128e98726b6cc8f36410/sc.py#L185

- Opt in registers dapp/user.
  - As part of opt in, the address of the entity and the lsig are stored in global state after validations.
  - Payment of a prescribed fee is validated here
- Public notification is written to the local state of dapp.
- Private notification is written to the local state of user.
- Verification updates the global state of the smart contract for the verified dapp.

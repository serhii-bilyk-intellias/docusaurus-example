---
sidebar_position: 1
---

# Key generation

Emulate operates **two completely isolated environments:** a stage (testing) environment and a production environment. The keys are not shared between them; nor are devices, customers, facilities, etc.

You can generate a public/private key pair in the Emulate portal. After the key generation you will be provided with the private part of the key, needed for JWT signing, and Emulate shall only retain the public part. To do this:

1. Log in to the Emulate portal, on either the stage environment or the production environment.
2. Go to the API Settings section of the portal.
3. Go to the Key Management tab.
4. It is possible to generate and register keys for different APIs. **Make sure you perform the following steps in the Single Customer API section, since this is the API used by the Emulate Web App**.
5. Locate the Generate Key Pair form. Enter a name for the key, for example "Web App Access". Press the Generate button.
6. The generated private key will be displayed. **You must save this; it is not saved by Emulate for security reasons, and thus cannot be displayed again.** You will need this private key for signing JWTs.
7. The public part of the key will have been saved by Emulate, and the name of the key, along with its creation date, will now be displayed in the Existing Keys table.
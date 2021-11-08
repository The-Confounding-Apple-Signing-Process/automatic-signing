# Automatic Signing

## Nuke all

- Remove all profiles in "/Users/uday/Library/MobileDevice/Provisioning Profiles"
- Remove all certificates and private keys in Keychain Access
- Remove all certificates and profiles in Apple Developer Portal

## Build using xCode

- Ensure that we are logged in user account in xCode.
- Ensure that project is set for "Automatic Signing".
- Ensure that correct Team is selected in xCode.
- Build for a device.
- Check Keychain Access and profiles path locally to verify xCode created developer certificates and profiles.
- Build for Archive.
- Verify xCode prompts to create distribution certificate.
- Check Keychain Access and profiles path locally to verify xCode created distribution certificates and profiles.

## Build using pipeline

- Ensure that we are logged in user account in xCode.
- Verify distribution certificate is present in Keychain Access.
- Remove all profiles in "/Users/uday/Library/MobileDevice/Provisioning Profiles"
- Build using pipeline.
- Check profiles path locally to verify xCode created distribution profiles using previously stored private key.


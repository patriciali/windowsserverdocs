---
title: Security Options
ms.custom: na
ms.prod: windows-server-2012
ms.reviewer: na
ms.suite: na
ms.technology: 
  - techgroup-security
ms.tgt_pltfrm: na
ms.topic: article
ms.assetid: e9fc52ee-b8b3-46ab-981f-4124b09a301b
---
# Security Options
This reference topic for the IT professional provides an introduction to the settings under **Security Options** of the local security policies and links to information about each setting.  
  
The **Security Options** contain the following groupings of security policy settings that allow you to configure the behavior of the local computer. Some of these policies can be included in a Group Policy Object and distributed over your enterprise.  
  
If you edit policy settings locally on a computer, you will affect the settings on only that one computer. If you configure the settings in a Group Policy Object \(GPO\) hosted in an Active Directory domain, the settings apply to all computers that are subject to that GPO. For more information about Group Policy in an Active Directory domain, see [Group Policy](http://go.microsoft.com/fwlink/?LinkId=55625)\(http:\/\/go.microsoft.com\/fwlink\/?LinkId\=55625\).  
  
For information about how the security policy snap\-in and related technologies work, see [Security Policy Settings Technical Overview](security-policy-settings-technical-overview.md).  
  
Open the Local Security Policy snap\-in \(secpol.msc\) and navigate to **Computer Configuration\\Windows Settings\\Security Settings\\Local Policies\\Security Options**.  
  
Local computer permissions: Membership in the local Administrators group, or equivalent, is the minimum required to modify these policy settings.  
  
For information about setting security policies, see [How to Configure Security Policy Settings](how-configure-security-policy-settings.md).  
  
|Grouping|Security Policy setting|  
|------------|---------------------------|  
|Accounts|-   [Accounts: Administrator account status](accounts-administrator-account-status.md)<br />-   [Accounts: Block Microsoft accounts](accounts-block-microsoft-accounts.md)<br />-   [Accounts: Guest account status](accounts-guest-account-status.md)<br />-   [Accounts: Limit local account use of blank passwords to console logon only](accounts-limit-local-account-use-blank-passwords-console-logon-only.md)<br />-   [Accounts: Rename administrator account](accounts-rename-administrator-account.md)<br />-   [Accounts: Rename guest account](accounts-rename-guest-account.md)|  
|Audit|-   [Audit: Audit the access of global system objects](audit-audit-access-global-system-objects.md)<br />-   [Audit: Audit the use of Backup and Restore privilege](audit-audit-use-backup-restore-privilege.md)<br />-   [Audit: Force audit policy subcategory settings &#40;Windows Vista or later&#41; to override audit policy category settings]()<br />-   [Audit: Shut down system immediately if unable to log security audits](audit-shut-down-system-immediately-unable-log-security-audits.md)|  
|DCOM|-   [DCOM: Machine Access Restrictions in Security Descriptor Definition Language &#40;SDDL&#41; syntax](../../../group-managed-service-accounts/manage/reference/security-options/dcom-machine-access-restrictions-security-descriptor-definition-language-sddl-syntax.md)<br />-   [DCOM: Machine Launch Restrictions in Security Descriptor Definition Language &#40;SDDL&#41; syntax](../../../group-managed-service-accounts/manage/reference/security-options/dcom-machine-launch-restrictions-security-descriptor-definition-language-sddl-syntax.md)|  
|Devices|-   [Devices: Allow undock without having to log on](devices-allow-undock-without-having-log-on.md)<br />-   [Devices: Allowed to format and eject removable media](devices-allowed-format-eject-removable-media.md)<br />-   [Devices: Prevent users from installing printer drivers](devices-prevent-users-from-installing-printer-drivers.md)<br />-   [Devices: Restrict CD-ROM access to locally logged-on user only](devices-restrict-cdrom-access-locally-loggedon-user-only.md)<br />-   [Devices: Restrict floppy access to locally logged-on user only](devices-restrict-floppy-access-locally-loggedon-user-only.md)|  
|Domain controller|-   [Domain controller: Allow server operators to schedule tasks](domain-controller-allow-server-operators-schedule-tasks.md)<br />-   [Domain controller: LDAP server signing requirements](domain-controller-ldap-server-signing-requirements.md)<br />-   [Domain controller: Refuse machine account password changes](domain-controller-refuse-machine-account-password-changes.md)|  
|Domain member|-   [Domain member: Digitally encrypt or sign secure channel data &#40;always&#41;](domain-member-digitally-encrypt-sign-secure-channel-data-always.md)<br />-   [Domain member: Digitally encrypt secure channel data &#40;when possible&#41;](domain-member-digitally-encrypt-secure-channel-data-when-possible.md)<br />-   [Domain member: Digitally sign secure channel data &#40;when possible&#41;](domain-member-digitally-sign-secure-channel-data-when-possible.md)<br />-   [Domain member: Disable machine account password changes](domain-member-disable-machine-account-password-changes.md)<br />-   [Domain member: Maximum machine account password age](domain-member-maximum-machine-account-password-age.md)<br />-   [Domain member: Require strong &#40;Windows 2000 or later&#41; session key](domain-member-require-strong-windows-2000-later-session-key.md)|  
|Interactive logon|-   [Interactive logon: Display user information when the session is locked](interactive-logon-display-user-information-when-session-locked.md)<br />-   [Interactive logon: Do not display last user name](interactive-logon-not-display-last-user-name.md)<br />-   [Interactive logon: Do not require CTRL+ALT+DEL](interactive-logon-not-require-ctrlaltdel.md)<br />-   [Interactive logon: Machine account lockout threshold](interactive-logon-machine-account-lockout-threshold.md)<br />-   [Interactive logon: Machine inactivity limit](interactive-logon-machine-inactivity-limit.md)<br />-   [Interactive logon: Message text for users attempting to log on](interactive-logon-message-text-users-attempting-log-on.md)<br />-   [Interactive logon: Message title for users attempting to log on](interactive-logon-message-title-users-attempting-log-on.md)<br />-   [Interactive logon: Number of previous logons to cache &#40;in case domain controller is not available&#41;](../../../group-managed-service-accounts/manage/reference/security-options/interactive-logon-number-previous-logons-cache-case-domain-controller-not-available.md)<br />-   [Interactive logon: Prompt user to change password before expiration](interactive-logon-prompt-user-change-password-before-expiration.md)<br />-   [Interactive logon: Require Domain Controller authentication to unlock workstation](interactive-logon-require-domain-controller-authentication-unlock-workstation.md)<br />-   [Interactive logon: Require smart card](interactive-logon-require-smart-card.md)<br />-   [Interactive logon: Smart card removal behavior](interactive-logon-smart-card-removal-behavior.md)|  
|Microsoft network client|-   [Microsoft network client: Digitally sign communications &#40;always&#41;](microsoft-network-client-digitally-sign-communications-always.md)<br />-   [Microsoft network client: Digitally sign communications &#40;if server agrees&#41;](microsoft-network-client-digitally-sign-communications-server-agrees.md)<br />-   [Microsoft network client: Send unencrypted password to third-party SMB servers](microsoft-network-client-send-unencrypted-password-thirdparty-smb-servers.md)|  
|Microsoft network server|-   [Microsoft network server: Amount of idle time required before suspending session](microsoft-network-server-amount-idle-time-required-before-suspending-session.md)<br />-   [Microsoft network server: Attempt S4U2Self to obtain claim information](microsoft-network-server-attempt-s4u2self-obtain-claim-information.md)<br />-   [Microsoft network server: Digitally sign communications &#40;always&#41;](microsoft-network-server-digitally-sign-communications-always.md)<br />-   [Microsoft network server: Digitally sign communications &#40;if client agrees&#41;](microsoft-network-server-digitally-sign-communications-client-agrees.md)<br />-   [Microsoft network server: Disconnect clients when logon hours expire](microsoft-network-server-disconnect-clients-when-logon-hours-expire.md)<br />-   [Microsoft network server: Server SPN target name validation level](microsoft-network-server-server-spn-target-name-validation-level.md)|  
|Network access|-   [Network access: Allow anonymous SID Name translation](network-access-allow-anonymous-sid-name-translation.md)<br />-   [Network access: Do not allow anonymous enumeration of SAM accounts](network-access-not-allow-anonymous-enumeration-sam-accounts.md)<br />-   [Network access: Do not allow anonymous enumeration of SAM accounts and shares](network-access-not-allow-anonymous-enumeration-sam-accounts-shares.md)<br />-   [Network access: Do not allow storage of passwords and credentials for network authentication](../../../group-managed-service-accounts/manage/reference/security-options/network-access-not-allow-storage-passwords-credentials-network-authentication.md)<br />-   [Network access: Let Everyone permissions apply to anonymous users](network-access-let-everyone-permissions-apply-anonymous-users.md)<br />-   [Network access: Named Pipes that can be accessed anonymously](network-access-named-pipes-that-can-accessed-anonymously.md)<br />-   [Network access: Remotely accessible registry paths](network-access-remotely-accessible-registry-paths.md)<br />-   [Network access: Remotely accessible registry paths and subpaths](network-access-remotely-accessible-registry-paths-subpaths.md)<br />-   [Network access: Restrict anonymous access to Named Pipes and Shares](assetId:///006b587e-9ca1-426c-8a0f-914fc283124c)<br />-   [Network access: Shares that can be accessed anonymously](network-access-shares-that-can-accessed-anonymously.md)<br />-   [Network access: Sharing and security model for local accounts](network-access-sharing-security-model-local-accounts.md)|  
|Network security|-   [Network security: Allow Local System to use computer identity for NTLM](network-security-allow-local-system-use-computer-identity-ntlm.md)<br />-   [Network security: Allow LocalSystem NULL session fallback](network-security-allow-localsystem-null-session-fallback.md)<br />-   [Network Security: Allow PKU2U authentication requests to this computer to use online identities](../../../group-managed-service-accounts/manage/reference/security-options/network-security-allow-pku2u-authentication-requests-this-computer-use-online-identities.md)<br />-   [Network security: Configure encryption types allowed for Kerberos](network-security-configure-encryption-types-allowed-kerberos.md)<br />-   [Network security: Do not store LAN Manager hash value on next password change](network-security-not-store-lan-manager-hash-value-next-password-change.md)<br />-   [Network security: Force logoff when logon hours expire](network-security-force-logoff-when-logon-hours-expire.md)<br />-   [Network security: LAN Manager authentication level](network-security-lan-manager-authentication-level.md)<br />-   [Network security: LDAP client signing requirements](network-security-ldap-client-signing-requirements.md)<br />-   [Network security: Minimum session security for NTLM SSP based &#40;including secure RPC&#41; clients](../../../group-managed-service-accounts/manage/reference/security-options/network-security-minimum-session-security-ntlm-ssp-based-including-secure-rpc-clients.md)<br />-   [Network security: Minimum session security for NTLM SSP based &#40;including secure RPC&#41; servers](../../../group-managed-service-accounts/manage/reference/security-options/network-security-minimum-session-security-ntlm-ssp-based-including-secure-rpc-servers.md)<br />-   [Network security: Restrict NTLM: Add remote server exceptions for NTLM authentication](../../../group-managed-service-accounts/manage/reference/security-options/network-security-restrict-ntlm-add-remote-server-exceptions-ntlm-authentication.md)<br />-   [Network security: Restrict NTLM: Add server exceptions in this domain](network-security-restrict-ntlm-add-server-exceptions-this-domain.md)<br />-   [Network Security: Restrict NTLM: Incoming NTLM Traffic](network-security-restrict-ntlm-incoming-ntlm-traffic.md)<br />-   [Network Security: Restrict NTLM: NTLM authentication in this domain](network-security-restrict-ntlm-ntlm-authentication-this-domain.md)<br />-   [Network Security: Restrict NTLM: Outgoing NTLM traffic to remote servers](network-security-restrict-ntlm-outgoing-ntlm-traffic-remote-servers.md)<br />-   [Network Security: Restrict NTLM: Audit Incoming NTLM Traffic](network-security-restrict-ntlm-audit-incoming-ntlm-traffic.md)<br />-   [Network Security: Restrict NTLM: Audit NTLM authentication in this domain](network-security-restrict-ntlm-audit-ntlm-authentication-this-domain.md)|  
|Recovery console|-   [Recovery console: Allow automatic administrative logon](recovery-console-allow-automatic-administrative-logon.md)<br />-   [Recovery console: Allow floppy copy and access to all drives and folders](recovery-console-allow-floppy-copy-access-all-drives-folders.md)|  
|Shutdown|-   [Shutdown: Allow system to be shut down without having to log on](shutdown-allow-system-shut-down-without-having-log-on.md)<br />-   [Shutdown: Clear virtual memory pagefile](shutdown-clear-virtual-memory-pagefile.md)|  
|System cryptography|-   [System cryptography: Force strong key protection for user keys stored on the computer](../../../group-managed-service-accounts/manage/reference/security-options/system-cryptography-force-strong-key-protection-user-keys-stored-computer.md)<br />-   [System cryptography: Use FIPS compliant algorithms for encryption, hashing, and signing](System-cryptography--Use-FIPS-compliant-algorithms-for-encryption,-hashing,-and-signing.md)|  
|System objects|-   [System objects: Require case insensitivity for non-Windows subsystems](system-objects-require-case-insensitivity-nonwindows-subsystems.md)<br />-   [System objects: Strengthen default permissions of internal system objects &#40;e.g. Symbolic Links&#41;](../../../group-managed-service-accounts/manage/reference/security-options/system-objects-strengthen-default-permissions-internal-system-objects-eg-symbolic-links.md)|  
|System settings|-   [System settings: Optional subsystems](system-settings-optional-subsystems.md)<br />-   [System settings: Use Certificate Rules on Windows Executables for Software Restriction Policies](../../../group-managed-service-accounts/manage/reference/security-options/system-settings-use-certificate-rules-windows-executables-software-restriction-policies.md)|  
|User Account Control|-   [User Account Control: Admin Approval Mode for the Built-in Administrator account](user-account-control-admin-approval-mode-builtin-administrator-account.md)<br />-   [User Account Control: Allow UIAccess applications to prompt for elevation without using the secure desktop](User-Account-Control--Allow-UIAccess-applications-to-prompt-for-elevation-without-using-the-secure-desktop.md)<br />-   [User Account Control: Behavior of the elevation prompt for administrators in Admin Approval Mode](../../../group-managed-service-accounts/manage/reference/security-options/user-account-control-behavior-elevation-prompt-administrators-admin-approval-mode.md)<br />-   [User Account Control: Behavior of the elevation prompt for standard users](user-account-control-behavior-elevation-prompt-standard-users.md)<br />-   [User Account Control: Detect application installations and prompt for elevation](user-account-control-detect-application-installations-prompt-elevation.md)<br />-   [User Account Control: Only elevate executables that are signed and validated](user-account-control-only-elevate-executables-that-signed-validated.md)<br />-   [User Account Control: Only elevate UIAccess applications that are installed in secure locations](../../../group-managed-service-accounts/manage/reference/security-options/user-account-control-only-elevate-uiaccess-applications-that-installed-secure-locations.md)<br />-   [User Account Control: Run all administrators in Admin Approval Mode](user-account-control-run-all-administrators-admin-approval-mode.md)<br />-   [User Account Control: Switch to the secure desktop when prompting for elevation](user-account-control-switch-secure-desktop-when-prompting-elevation.md)<br />-   [User Account Control: Virtualize file and registry write failures to per-user locations](../../../group-managed-service-accounts/manage/reference/security-options/user-account-control-virtualize-file-registry-write-failures-peruser-locations.md)|  
  

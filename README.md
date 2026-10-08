LESS Launcher
An independent desktop launcher project for players who own Minecraft: Java Edition.
> **Status: In development — not publicly released.** This repository is a public information page for LES Launcher and its application registration review. It is not a claim that all features are complete or available to download.
About LESS Launcher
LES Launcher is a Windows desktop application under development. Its goal is to bring curated modpack installations, account management, skin previews, screenshots, and optional community features into one interface.
The visual direction focuses on adventure and exploration, with original cartoon-inspired scenery, a straw-hat motif, and dark, red, and gold accents.
Application name for registration: LESS Launcher
Platform and stack: Windows · Electron · React · TypeScript · Vite · Supabase (for separate LES community accounts).
Current development status
Feature	Status
Desktop user interface	Development build available for internal testing
Local skin import and interactive 3D preview	Implemented in the development build; further testing ongoing
Separate LES account registration	Integrated with Supabase; testing ongoing
Community friend requests	Under development and testing
Modpack library	Interface in development; installation and game launch are not yet operational
Official Microsoft sign-in and Minecraft account verification	Integration in progress; Minecraft Services access currently blocked pending app registration review
Screenshots and customization	Under development
This table describes development progress, not a finished public product.
Why official Minecraft Services access is needed
LESS Launcher intends to authenticate legitimate Minecraft: Java Edition users through Microsoft's official browser-based authorization flow and the appropriate Xbox/Minecraft Services endpoints.
If the required application approval is granted, the planned authentication flow will:
Let users authorize sign-in on an official Microsoft page, rather than entering their Microsoft password into LES Launcher.
Obtain authorized tokens using a secure desktop OAuth flow with PKCE.
Perform the required official Minecraft account and license/entitlement checks before enabling licensed game launching.
Retrieve the authenticated player's Minecraft username, UUID, and skin metadata for their launcher profile.
Support secure session handling, token expiration, and sign-out.
Registration review status: During development, the Minecraft authentication integration returned `HTTP 403 — Invalid app registration` at the Minecraft Services stage. We are seeking review/approval of the LES Launcher application ID. We do not claim that Minecraft account authentication or game launch works until the integration is authorized and successfully tested.
Security and compliance commitments
LESS Launcher is intended for users who have legitimate access to Minecraft: Java Edition.
The launcher will not bypass, disable, or weaken authentication, account-security controls, licensing/ownership checks, or other required safety features.
LESS Launcher will not request, collect, or store Microsoft account passwords.
Separate LES community accounts provided through Supabase are for launcher/community features only. They do not grant access to Minecraft or replace the official Microsoft authentication and game-license requirements.
Any local profile or offline UI preview functionality is for launcher customization/testing only, not a mechanism for bypassing official Minecraft licensing or protected server authentication.
Authentication-related functions will remain restricted until the appropriate approvals, permissions, and tests are complete.
Project availability
LES Launcher is currently being tested privately on Windows. A public download and setup guide will be published only when essential features and security requirements are ready. This repository is currently for project information, not distribution.
Contact
For general questions about the project, open a GitHub Issue in this repository. For an application registration request, the applicant will provide a valid direct contact email in the official review form.
Unofficial project disclaimer
LES Launcher is an independent, unofficial application and is not affiliated with, sponsored by, or endorsed by Microsoft, Mojang Studios, or Minecraft. All third-party names and trademarks belong to their respective owners. Their mention here describes technical compatibility and authentication requirements, not the name of this application or an endorsement.

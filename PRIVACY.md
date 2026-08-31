# Privacy Policy for Capture by TyD

**Effective date:** August 31, 2026  
**Publisher:** YSProductions / TyD

Capture by TyD ("Capture") is a Windows desktop application for taking screenshots, recording instant replays, editing saved media, recognizing text in screenshots, and optionally sharing captures through services configured by the user.

## Summary

Capture does not include advertising, developer analytics, or telemetry. Capture does not automatically send screenshots, recordings, microphone audio, OCR text, or diagnostic logs to the developer. Media remains on the user's device unless the user chooses to share it through a service they configure.

## Information processed locally

Depending on the features the user enables, Capture may process and store:

- screenshots and screen or game recordings;
- game or application names and process information used to select a capture target;
- game/system audio, optional Discord process audio (including call participant voices and other Discord sounds), and microphone audio included in recordings;
- locally recognized text from screenshots for library search;
- capture metadata, thumbnails, edit/export settings, and public share URLs;
- application preferences, including capture locations, hotkeys, audio-device selections, and sharing configuration;
- operational logs containing app, encoder, file-path, device, and error information needed for troubleshooting.

These items are stored locally in the capture folder or Capture application-data folder selected or controlled by the user. Clipboard features place an image, file reference, or share URL on the Windows clipboard only when requested.

## Network activity and optional sharing

Microsoft Store builds use Microsoft Store services to install and update the application. Non-Store builds may check Capture's public Cloudflare R2 update feed. Like ordinary web requests, these providers may receive technical connection information such as IP address, request time, and user agent under their own privacy terms.

Capture can optionally connect to third-party services configured by the user:

- **Cloudflare R2 or another compatible S3 endpoint:** When the user chooses Upload or Share, Capture sends the selected media file to the bucket configured by that user. Capture stores the resulting object key and public URL locally. The user controls the bucket, retention, permissions, and public accessibility.
- **Discord webhook:** If enabled by the user, Capture sends the uploaded file's name and public share URL to the Discord channel represented by the configured webhook.

Capture does not provide the developer with the user's R2 credentials, Discord webhook, captures, or account information. R2 secret keys and Discord webhook URLs are encrypted using Electron's Windows secure storage before being saved locally. Users should review the privacy and retention practices of Microsoft, Cloudflare, Discord, or any alternative endpoint they configure.

## Retention and deletion

Local captures remain until the user deletes them or enables automatic cleanup. Users can change the capture folder, clear cached thumbnails, delete local captures, and request deletion of R2 objects that were uploaded through Capture. Deleting a local file does not guarantee deletion of copies previously shared, downloaded, reposted, backed up, or retained by a third-party service.

Application settings and logs remain in the user's Windows application-data folder until removed by the user or operating system. Uninstall behavior may retain application data so captures and preferences are not unexpectedly destroyed.

## Data sharing and sale

The developer does not sell personal information. Capture does not share personal information with advertisers or data brokers. Data is transmitted only as described above, when required for installation/update delivery, or when the user directs Capture to use a configured sharing service.

## Children

Capture is a general-purpose desktop utility and is not directed to children under 13. The developer does not knowingly collect children's personal information through Capture.

## Security

Capture uses Windows-provided secure storage for supported local secrets and HTTPS for configured network services. No software or transmission method can guarantee absolute security. Users are responsible for protecting their Windows account, webhook URLs, cloud credentials, public links, and configured storage services.

## Changes to this policy

This policy may be updated when Capture's behavior or legal requirements change. The effective date above will be revised, and the current version will remain available at this URL.

## Contact and privacy requests

For privacy questions, support, or deletion guidance, open a request through the [Capture legal support page](SUPPORT.md). Do not include passwords, cloud secret keys, Discord webhook URLs, private captures, or other sensitive information in a public issue.

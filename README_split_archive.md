# Split release archive

GitHub web upload rejects files larger than 25 MB. The submission reproducibility package was therefore split into 8 parts for browser upload.

Original ZIP:

- `repository_release_package_upload_candidate_v0.1.0-submission.zip`
- SHA256: `5c1eb853bbd18d8f662f03c9bb5d1a2925325aa142b8d307ed60daeb6d030e83`

Reassemble on Windows PowerShell from this folder:

```powershell
$parts = Get-ChildItem -Filter "repository_release_package_upload_candidate_v0.1.0-submission.zip.part*" | Sort-Object Name
Get-Content -Encoding Byte -Path $parts.FullName | Set-Content -Encoding Byte -Path .\repository_release_package_upload_candidate_v0.1.0-submission.zip
Get-FileHash .\repository_release_package_upload_candidate_v0.1.0-submission.zip -Algorithm SHA256
```

The resulting SHA256 must match the original checksum above.

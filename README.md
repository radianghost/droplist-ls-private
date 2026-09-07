# Spamhaus DROP for LS

This repository republishes the official Spamhaus DROP IPv4 and IPv6 CIDR lists for use as LS blocklists.

## Add the lists to LS

Add each URL separately in the **Blocklists** section:

```text
https://raw.githubusercontent.com/radianghost/droplist-ls/main/drop_v4.txt
https://raw.githubusercontent.com/radianghost/droplist-ls/main/drop_v6.txt
```

These are plain CIDR blocklists. Do not add them as a Remote Rule Group, which expects a different `.lsrules` JSON format.

## Updates

The GitHub Action checks once daily at 06:17 UTC, but downloads and publishes only once every continuous three days. A manual Action run updates immediately.

Before publishing, the updater validates the official Spamhaus data and accepts only global IPv4 and IPv6 CIDR ranges. The two files are changed only when their contents differ.

## Privacy

The repository is public because LS needs to download these files without GitHub authentication. It contains no subscriber information or credentials.

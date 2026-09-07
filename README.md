# Update drop lists

```text
https://raw.githubusercontent.com/radianghost/droplist-ls/main/drop_v4.txt
https://raw.githubusercontent.com/radianghost/droplist-ls/main/drop_v6.txt
```

## Updates

The GitHub Action checks once daily at 06:17 UTC, but downloads and publishes only once every continuous three days. A manual Action run updates immediately.

Before publishing, the updater validates the official Spamhaus data and accepts only global IPv4 and IPv6 CIDR ranges. The two files are changed only when their contents differ.

---
functions:
  execute-interactive:
    - code: |
        TERM= more /etc/profile
        !/bin/sh
  file-read:
    - code: more file_to_read
  suid-enabled:
    - code: ./more file_to_read
  sudo-enabled:
    - code: |
        TERM= sudo -E more /etc/profile
        !/bin/sh
---

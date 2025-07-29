# Cyber Camp 2025 Cyber Defense Forensic Analyst (CDFA)

This repository contains useful files for the Cyber Defense Forensic Analyst activity in the 2025 **Cyber-Guardians Navigating the AI-Enhanced Future** summer camp at Fresno State.  

## Scenario

You've been hired into a Cyber Defense Forensic Analyst role at a cybersecurity company that performs incident response.  Three different clients (Companies A, B, and C) have had confirmed security incidents but they don't know if any data was stolen.  Their network traffic shows the only data that left each company's network were chat messages.  Your job is to analyze the chat logs and determine whether any company data was stolen.

Review the files in the three folders:

1. company_a
1. company_b
1. company_c

### Translation (tr)
The `tr` command can be used to perform direct conversion of characters for simple encryption such as the Caesar Cipher.  For example, to encrypt the text in a file with a +3 cipher:

```
tr "a-z" "d-zabc" < plaintext > ciphertext
```

To decrypt, simply reverse:

```
tr "d-zabc" "a-z" < ciphertext > decodedtext
```

### Steghide
The `steghide` program can be used for file steganography.  First, install steghide:

```
sudo apt install steghide -y
```

To embed *secret.txt* into *image.jpg* creating *steg_image.jpg*:

```
steghide embed -ef secret.txt -cf image.jpg -sf steg_image.jpg
```

To extract *secret.txt* from *steg_image.jpg*:

```
steghide extract -sf steg_image.jpg
```
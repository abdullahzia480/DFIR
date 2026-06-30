# Manual SYSKEY and PEK Reconstruction from Active Directory Artifacts

## Overview

This investigation documents the manual extraction and reconstruction of the Windows System Boot Key (SYSKEY) and the subsequent decryption and recovery of the Password Encryption Key (PEK) from Active Directory artifacts.

The objective of this analysis was to validate the internal cryptographic mechanisms used by Windows Active Directory by manually reconstructing the SYSKEY from registry hives, decrypting the PEK stored within `ntds.dit`, and verifying the results against automated forensic tools.

## Investigation Objectives

* Extract SYSKEY fragments from the SYSTEM registry hive.
* Manually reconstruct the Windows Boot Key.
* Verify the reconstructed key against DSInternals.
* Locate and extract the Password Encryption Key (PEK) from `ntds.dit`.
* Perform manual AES decryption of the PEK structure.
* Recover the raw symmetric key used by Active Directory.

## Tools Used

* Registry Explorer
* Hex Editor
* DSInternals
* ESE Database Viewer
* CyberChef
* Windows Registry Artifacts
* Active Directory Database (`ntds.dit`)

## Key Areas Covered

* Windows Registry Forensics
* Active Directory Internals
* SYSKEY Reconstruction
* PEK Decryption
* Hex-Level Artifact Analysis
* AES Cryptographic Analysis
* Credential Storage Architecture

## Files

* `Manual Extraction and Reconstruction of the Boot Key.pdf`  Complete technical investigation and forensic walkthrough.

## Disclaimer

This investigation was conducted for educational, research, and digital forensic purposes only.

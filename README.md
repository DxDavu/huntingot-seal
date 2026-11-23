# Sealed by Hunt · daily seals

This repository keeps a copy of every daily seal of the **Hunt Ingot** record book (https://huntingot.com/seal).
A GitHub Action adds one file a day, `days/<YYYY-MM-DD>.json`, fetched from `https://api.huntingot.com/v1/days/latest`.
Hunt cannot change a seal here without the change showing in this repository's history.

- Each file is a signed day root: the Merkle root of that day's hourly seals, the last line of every
  series book, Hunt's key id and its Ed25519 signature, and the other witnesses (Sigstore Rekor, an
  RFC 3161 time-stamp).
- Check any card at https://huntingot.com, or check a proof file at https://huntingot.com/check.
- Days with no card moves have no seal.

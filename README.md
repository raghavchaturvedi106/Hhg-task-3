# HH Goa 2026 Task 3: Face ID & Blockchain Verification Pipeline

## Overview
An end-to-end pipeline that takes a face scan as input, identifies matching content on social media/web, and anchors the discovered metadata onto a blockchain for tamper-evident verification.

## Pipeline Architecture
1. **Face Identification:** Uses `face_recognition` (dlib) to detect and extract face encodings from an input image.
2. **Social Media Search:** Searches the web/social media for matching profile posts using visual search algorithms.
3. **Blockchain Verification:** Generates a Keccak-256 fingerprint of the post data and anchors it on-chain with block confirmation and re-verification.

## How to Run
This project runs automatically via **GitHub Actions**:
1. Go to the **Actions** tab in this repository.
2. Select **Face-ID Blockchain Verification Pipeline**.
3. Click **Run workflow** -> **Run workflow**.
4. View the real-time execution logs showing face detection, post match, and blockchain transaction receipts.

## Known Limitations
- Social media rate limits may apply on dynamic API queries.
- Private social media profiles cannot be scraped directly without authentication.

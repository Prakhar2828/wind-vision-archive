# Wind VISION Historical Archive — CAS V1

## Archive contents
- 3,855 original file records
- 1,948 unique SHA-256-addressed objects
- 26 multipart TAR assets
- Original logical size: 35.378 GiB
- Deduplicated package: approximately 25.99 GiB

## Verification
- All 26 archive part checksums: PASS
- Every stored object's SHA-256: PASS
- Embedded original manifest: PASS
- Independent restoration of all 3,855 files: PASS

## Recovery notes
The 26 parts form a single content-addressed TAR stream.
They must be concatenated in filename order.

Simply extracting the TAR produces SHA-256-addressed blobs,
not the original directory tree. A CAS-aware restoration
procedure must use the embedded master manifest to reconstruct
the original paths and verify their file contents.

The original manifest contains 3,855 file records and is
embedded in the TAR stream.

## Remote backup status
Full remote upload: NOT COMPLETED
Full remote download and restoration: NOT TESTED

No bulk historical payload should be uploaded until its
security and external-storage authorization reviews are complete.

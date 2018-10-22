---
description: As an option, you can compress data files when sending them to Audience Manager.
seo-description: As an option, you can compress data files when sending them to Audience Manager.
seo-title: File Compression for Inbound Data Transfer Files
solution: Audience Manager
title: File Compression for Inbound Data Transfer Files
uuid: 03deb0d5-133b-4e24-9f58-00dfa218c4ce
index: y
internal: n
snippet: y
translate: y
---

# File Compression for Inbound Data Transfer Files

As an option, you can compress data files when sending them to Audience Manager.

<!-- inbound-file-compression.xml -->

Audience Manager supports gzip ( `.gz`) compression for inbound, asynchronous data transfers.

Audience Manager also supports uncompressed files.

>[!IMPORTANT]
>
>We currently don't support encryption and compression on the same inbound data file. You can select to either [encrypt](../../../c_integration/sending-audience-data/batch-data-transfer-explained/inbound-file-encryption.md#concept_94660DC77BAB4D558B793D59988B0A21) or compress your inbound files.

**Amazon S3 Compression**

For delivery to Amazon S3, you must use `.gz` or uncompressed files. Compressed files must be 1 GB or smaller. If the files are larger, please discuss the file and transfer process with Customer Care. Although [!DNL Audience Manager] can handle very large files, there may be ways to reduce the file size or make transfer of data more efficient.

>[!IMPORTANT]
>
>Your FTP client must use binary mode to transfer compressed or encrypted files. Compressed or encrypted files sent in ASCII mode will corrupt the data transfer file.

**Best Practices**

* Files should be gzip compressed (and have a [!DNL .gz] file extension.) 
* The maximum compressed file size for a `.gz` compressed file is 1 GB. 
* Optimal split sizes, for fastest/earliest processing of your files, is approximately 1 GB uncompressed or 200-300 MB compressed. 
* Amazon S3 imposes its own, 5 GB file size limit on uploaded files.

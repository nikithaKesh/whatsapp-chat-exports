# WhatsApp Archive Viewer v1.5

Open index.html in a browser, then import your WhatsApp TXT or ZIP archive.

## Search and calendar filtering
- Use **Search messages** to find words or phrases within message text, senders, or attachment filenames.
- Use **Search by date** to open your browser's calendar and display messages from a specific day.
- Combine both filters to find a particular word on a particular day.
- Click **Clear filters** to return to the full conversation. The date filter works with parsed dates in the imported WhatsApp export.
- The left sidebar's **Search conversations** still filters chat names.

## Reply links
Your sample WhatsApp export does **not** contain metadata identifying which messages were replies. This version does not invent reply relationships.

1. On an older message, click **Quote**.
2. Find the message that replied to it and click **Link reply**.
3. The reply gets a quoted preview. Click that preview to jump to the original message.
4. Use **Unlink** to remove a relationship.

Links are stored in your browser's localStorage, tied to a fingerprint of the exact imported transcript. They are not added to the exported archive and won't automatically move to another browser, device, or a changed export file. The original chat text remains untouched.

WhatsApp does not include reply-to metadata in many standard TXT exports. This sample ZIP contains 3,392 message records and 807 omitted-media indicators, but no detected reply metadata.

This is a read-only archive viewer. ZIP reading uses JSZip via CDN and requires connectivity.

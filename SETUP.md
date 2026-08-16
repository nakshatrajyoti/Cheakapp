# Nakshatra Jyoti V7 ULTRA

यह package मौजूदा 8K+ script.js को आधार बनाकर बनाया गया है।

मुख्य बात:
- पुराने script.js को replace नहीं किया गया; existing 8,667 lines preserved हैं और V7 feature layer नीचे जोड़ी गई है।
- User / Acharya / Admin role presentation अलग है।
- User Home: Poster -> आज का राशिफल -> सभी 12 राशियों के अलग boxes -> guidance.
- राशिफल का सही शब्द अब `राशिफल` है।
- Acharya/Admin के लिए role-specific workspace.
- User स्वयं को message/call नहीं कर सकता; Acharya अपने आप को message नहीं कर सकता।
- Realtime chat/presence के लिए existing Firebase onSnapshot layer preserved है और V7 presentation enhancement जोड़ा गया है।
- Admin notification/rashifal/poster controls existing system के साथ preserved हैं।
- Dark theme, command palette, premium cards, filters, back navigation helpers और responsive presentation जोड़े गए हैं।

Firebase:
`firebase-config.js` में अपना वास्तविक Web App config रखें।
Firestore/Storage rules को Firebase Console में deploy करें।

महत्वपूर्ण:
Browser UI से किसी User को Admin बनाना सुरक्षित नहीं है। Admin role server-side/Firestore rules से नियंत्रित रखें।


## V8 PRO additions
- Built directly on V7 ULTRA FULL.
- Full-screen messages with fixed header, back button and no bottom navigation while chatting.
- Own-message deletion for users and acharyas (rules updated).
- Conversation unread badge is conversation-level: always 1 per unread conversation.
- Message notifications are written to the recipient notification center.
- Acharya self profile editing; Admin can manage authorized Acharya profiles.
- Gallery photo selection with crop/zoom/pan/rotate; video selection and web playback.
- Instagram-style Acharya profile with post count, feed, Instagram/Facebook links.
- Posts support likes, comments, image/video media, author deletion.
- Acharya/Admin Rashifal publishing.

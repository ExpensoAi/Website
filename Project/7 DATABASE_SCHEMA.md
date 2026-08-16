# EXPENSO AI WEBSITE
# DATABASE SCHEMA

Version: 1.0

---

# 1. USERS

users

Fields:

id
email
name
avatar_url
auth_provider
role
status
created_at
updated_at
last_login_at

Roles:

user
premium_user
moderator
support_agent
admin
super_admin

---

# 2. SUPPORT TICKETS

support_tickets

Fields:

id
ticket_number
user_id
category
priority
subject
description
status
assigned_agent_id
created_at
updated_at
resolved_at
closed_at

---

# 3. SUPPORT MESSAGES

support_messages

Fields:

id
ticket_id
sender_id
message
is_internal
created_at

---

# 4. SUPPORT ATTACHMENTS

support_attachments

Fields:

id
ticket_id
message_id
file_name
file_type
file_size
storage_path
created_at

Files must not be publicly accessible.

---

# 5. COMMUNITY POSTS

community_posts

Fields:

id
user_id
category_id
title
content
status
created_at
updated_at

---

# 6. COMMUNITY COMMENTS

community_comments

Fields:

id
post_id
user_id
parent_comment_id
content
status
created_at
updated_at

---

# 7. COMMUNITY VOTES

community_votes

Fields:

id
post_id
user_id
created_at

A user should not be able to vote multiple times for the same item unless explicitly supported.

---

# 8. COMMUNITY REPORTS

community_reports

Fields:

id
reporter_id
post_id
comment_id
reason
description
status
reviewed_by
created_at
reviewed_at

---

# 9. FEATURE REQUESTS

feature_requests

Fields:

id
user_id
title
description
category
status
vote_count
created_at
updated_at
released_at

---

# 10. FEATURE REQUEST VOTES

feature_request_votes

Fields:

id
feature_request_id
user_id
created_at

---

# 11. BUG REPORTS

bug_reports

Fields:

id
user_id
title
description
steps_to_reproduce
expected_behavior
actual_behavior
device
android_version
app_version
priority
status
created_at
updated_at
resolved_at

---

# 12. KNOWLEDGE BASE

knowledge_articles

Fields:

id
category_id
title
slug
summary
content
status
author_id
created_at
updated_at
published_at

---

# 13. KNOWLEDGE CATEGORIES

knowledge_categories

Fields:

id
name
description
slug
sort_order

---

# 14. ANNOUNCEMENTS

announcements

Fields:

id
title
content
status
author_id
published_at
created_at
updated_at

---

# 15. RELEASE NOTES

release_notes

Fields:

id
version
title
summary
content
release_date
status
created_at

---

# 16. NOTIFICATIONS

notifications

Fields:

id
user_id
type
title
message
reference_type
reference_id
is_read
created_at

---

# 17. BOOKMARKS

bookmarks

Fields:

id
user_id
content_type
content_id
created_at

---

# 18. AUDIT LOG

audit_logs

Fields:

id
admin_id
action
entity_type
entity_id
old_value
new_value
created_at

Sensitive data must not be stored unnecessarily.

---

# 19. DATABASE RULES

All relationships must use foreign keys.

Use indexes for:

- user_id
- created_at
- status
- category
- ticket_number
- slug

Use unique constraints where required.

Use migrations for schema changes.
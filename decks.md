# Email
;ty;Thank you;Thank you for your message. I will get back to you shortly.
;sig;Email Signature;Best regards,\n{{clipboard}}
;ack;Acknowledge Receipt;Thank you for sending this over. I have received it and will review it shortly.
;followup;Follow Up;I wanted to follow up on my previous message. Please let me know if you have any questions or need further information.
;ooo;Out of Office;I am currently out of the office and will return on {{input:return_date}}. For urgent matters, please contact {{input:backup_contact}}.

# Customer Support
;sorry;Apology;I sincerely apologize for the inconvenience. Let me look into this for you right away.
;resolved;Issue Resolved;I have resolved the issue you reported. Please let me know if you experience any further problems.
;escalate;Escalate Issue;I am escalating this to our specialist team for further investigation. You will hear back within {{input:timeframe|24 hours}}.

# Development
;pr;PR Description;## Summary\n{{input:summary}}\n\n## Changes\n- {{input:changes}}\n\n## Testing\n- {{input:testing}}
;todo;TODO Comment;// TODO: {{input:description}} - {{username}} {{date}}
;fixme;FIXME Comment;// FIXME: {{input:description}} - {{username}} {{date}}
;log;Console Log;console.log('{{input:label}}:', {{clipboard}});
;dbg;Debug Print;Debug.WriteLine($"{{input:label}}: {{{clipboard}}}");

# Meetings
;agenda;Meeting Agenda;Meeting Agenda - {{date}}\n\nAttendees: {{input:attendees}}\n\n1. {{input:topic_1}}\n2. {{input:topic_2}}\n3. Action items review\n4. Next steps
;minutes;Meeting Minutes;Meeting Minutes - {{date}}\n\nAttendees: {{input:attendees}}\n\nDiscussion:\n{{input:notes}}\n\nAction Items:\n- {{input:actions}}\n\nNext Meeting: {{input:next_date}}

# Productivity
;now;Current Timestamp;{{datetime}}
;uuid;Generate UUID;{{guid}}
;clip;Clipboard Wrapper;{{clipboard}}

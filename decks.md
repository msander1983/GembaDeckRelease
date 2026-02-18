# Email
ty;Thank You;Thank you for your message. I will get back to you shortly.
sig;Email Signature;Best regards,\n{{clipboard}}
ack;Acknowledge Receipt;Thank you for sending this over. I have received it and will review it shortly.
followup;Follow Up;I wanted to follow up on my previous message. Please let me know if you have any questions or need further information.
ooo;Out of Office;I am currently out of the office and will return on {{input:return_date}}. For urgent matters, please contact {{input:backup_contact}}.
intro;Introduction;Hi {{input:name}},\n\nI wanted to introduce myself. I'm {{username}}, and I {{input:role_context}}. Looking forward to working with you.
decline;Polite Decline;Thank you for reaching out. Unfortunately, I'm unable to accommodate this request at this time. I appreciate your understanding.
confirm;Confirm Meeting;This is to confirm our meeting on {{input:date}} at {{input:time}}. Please let me know if this still works for you.
delay;Delay Notice;I wanted to let you know that {{input:item}} has been delayed. The new expected date is {{input:new_date}}. I apologize for the inconvenience.
referral;Referral;Thank you for your inquiry. I'm looping in {{input:colleague}} who is better positioned to help with this. {{input:colleague}}, could you please assist?
recap;Email Recap;Hi all,\n\nHere's a quick recap of our discussion:\n\n{{input:key_points}}\n\nNext steps:\n{{input:next_steps}}\n\nPlease let me know if I missed anything.
urgent;Urgent Request;Hi {{input:name}},\n\nThis requires your immediate attention. {{input:details}}\n\nPlease respond at your earliest convenience.
welcome;Welcome Email;Welcome to the team, {{input:name}}! We're excited to have you on board. Your first day details: {{input:details}}\n\nDon't hesitate to reach out if you have any questions.
feedback-req;Request Feedback;Hi {{input:name}},\n\nI'd appreciate your feedback on {{input:topic}}. If you could share your thoughts by {{input:deadline}}, that would be great.

# Customer Support
sorry;Apology;I sincerely apologize for the inconvenience. Let me look into this for you right away.
resolved;Issue Resolved;I have resolved the issue you reported. Please let me know if you experience any further problems.
escalate;Escalate Issue;I am escalating this to our specialist team for further investigation. You will hear back within {{input:timeframe|24 hours}}.
refund;Refund Confirmation;Your refund of {{input:amount}} has been processed. Please allow {{input:timeframe|5-7 business days}} for it to appear in your account.
eta;ETA Response;Thank you for your patience. The estimated resolution time is {{input:eta}}. I will keep you updated on progress.
workaround;Workaround;While we work on a permanent fix, here is a workaround you can try:\n\n{{input:steps}}
closed;Ticket Closed;This support ticket has been closed. If you need further assistance, please don't hesitate to reopen it or create a new request.
greeting;Support Greeting;Hello {{input:name}}, thank you for contacting support. My name is {{username}}, and I'll be assisting you today. How can I help?
faq;FAQ Response;Great question! {{input:answer}}\n\nFor more details, please see our help article: {{input:link}}
csat;Satisfaction Follow-Up;We hope your issue has been resolved. We'd love to hear your feedback — how was your experience? Your input helps us improve.
known-issue;Known Issue;Thank you for reporting this. We're aware of this issue and our team is actively working on a fix. We expect it to be resolved by {{input:eta}}.

# Development
pr;PR Description;## Summary\n{{input:summary}}\n\n## Changes\n- {{input:changes}}\n\n## Testing\n- {{input:testing}}
todo;TODO Comment;// TODO: {{input:description}} - {{username}} {{date}}
fixme;FIXME Comment;// FIXME: {{input:description}} - {{username}} {{date}}
log;Console Log;console.log('{{input:label}}:', {{clipboard}});
dbg;Debug Print;Debug.WriteLine($"{{input:label}}: {{{clipboard}}}");
hack;Hack Comment;// HACK: {{input:reason}} - {{username}} {{date}}\n// This should be refactored when {{input:condition}}
trycatch;Try-Catch Block;try\n{\n    {{clipboard}}\n}\ncatch (Exception ex)\n{\n    // TODO: Handle exception\n    throw;\n}
region;Region Block;#region {{input:name}}\n{{clipboard}}\n#endregion
xmldoc;XML Doc Comment;/// <summary>\n/// {{input:description}}\n/// </summary>
jsdoc;JSDoc Comment;/**\n * {{input:description}}\n * @param {{{input:param_type}}} {{input:param_name}} - {{input:param_desc}}\n * @returns {{{input:return_type}}} {{input:return_desc}}\n */
pydef;Python Function;def {{input:name}}({{input:params}}):\n    """{{input:description}}"""\n    {{clipboard}}
csmethod;C# Method;public {{input:return_type}} {{input:name}}({{input:params}})\n{\n    {{clipboard}}\n}
test;Unit Test;[Fact]\npublic void {{input:method}}_{{input:scenario}}_{{input:expected}}()\n{\n    // Arrange\n    {{input:arrange}}\n\n    // Act\n    {{input:act}}\n\n    // Assert\n    {{input:assert}}\n}
bench;Benchmark Timer;var sw = System.Diagnostics.Stopwatch.StartNew();\n{{clipboard}}\nsw.Stop();\nConsole.WriteLine($"Elapsed: {sw.ElapsedMilliseconds}ms");
null;Null Check;ArgumentNullException.ThrowIfNull({{input:param}});
guard;Guard Clause;if ({{input:condition}})\n    throw new {{input:exception|ArgumentException}}("{{input:message}}");
dispose;Dispose Pattern;public void Dispose()\n{\n    Dispose(true);\n    GC.SuppressFinalize(this);\n}\n\nprotected virtual void Dispose(bool disposing)\n{\n    if (disposing)\n    {\n        {{clipboard}}\n    }\n}
singleton;Singleton Property;private static readonly Lazy<{{input:type}}> _instance = new(() => new {{input:type}}());\npublic static {{input:type}} Instance => _instance.Value;

# Git & CI
gitco;Git Commit (Conventional);{{input:type|feat}}: {{input:description}}\n\n{{input:body}}
gitbr;Git Branch Name;{{input:type|feature}}/{{input:ticket}}-{{input:slug}}
gitpr-fix;Bug Fix PR;## Bug Fix\n\n**Problem:** {{input:problem}}\n**Root Cause:** {{input:cause}}\n**Fix:** {{input:fix}}\n\n## Testing\n- {{input:testing}}
gitcl;Changelog Entry;## [{{input:version}}] - {{date}}\n### Added\n- {{input:added}}\n### Changed\n- {{input:changed}}\n### Fixed\n- {{input:fixed}}
cienv;CI Environment Variable;env:\n  {{input:name}}: ${{ secrets.{{input:secret_name}} }}
gha;GitHub Action Step;- name: {{input:name}}\n  run: {{input:command}}

# Meetings
agenda;Meeting Agenda;Meeting Agenda - {{date}}\n\nAttendees: {{input:attendees}}\n\n1. {{input:topic_1}}\n2. {{input:topic_2}}\n3. Action items review\n4. Next steps
minutes;Meeting Minutes;Meeting Minutes - {{date}}\n\nAttendees: {{input:attendees}}\n\nDiscussion:\n{{input:notes}}\n\nAction Items:\n- {{input:actions}}\n\nNext Meeting: {{input:next_date}}
standup;Standup Update;**Yesterday:** {{input:yesterday}}\n**Today:** {{input:today}}\n**Blockers:** {{input:blockers|None}}
retro;Retrospective;## Retrospective - {{date}}\n\n**What went well:**\n- {{input:good}}\n\n**What could improve:**\n- {{input:improve}}\n\n**Action items:**\n- {{input:actions}}
1on1;1:1 Notes;## 1:1 with {{input:name}} - {{date}}\n\n**Updates:**\n{{input:updates}}\n\n**Discussion:**\n{{input:discussion}}\n\n**Action Items:**\n- {{input:actions}}
decision;Decision Record;## Decision: {{input:title}}\n**Date:** {{date}}\n**Status:** {{input:status|Accepted}}\n\n**Context:** {{input:context}}\n**Decision:** {{input:decision}}\n**Consequences:** {{input:consequences}}

# Productivity
now;Current Timestamp;{{datetime}}
uuid;Generate UUID;{{guid}}
clip;Clipboard Wrapper;{{clipboard}}
hr;Horizontal Rule;---
h1;Heading 1;# {{input:title}}
h2;Heading 2;## {{input:title}}
h3;Heading 3;### {{input:title}}
bullet;Bullet List;- {{input:item_1}}\n- {{input:item_2}}\n- {{input:item_3}}
checkbox;Checkbox List;- [ ] {{input:item_1}}\n- [ ] {{input:item_2}}\n- [ ] {{input:item_3}}
table;Markdown Table;| {{input:col1}} | {{input:col2}} | {{input:col3}} |\n|---|---|---|\n| {{input:val1}} | {{input:val2}} | {{input:val3}} |
link;Markdown Link;[{{input:text}}]({{input:url}})
img;Markdown Image;![{{input:alt_text}}]({{input:url}})
codeblock;Code Block;```{{input:lang}}\n{{clipboard}}\n```
kbd;Keyboard Shortcut;<kbd>{{input:key}}</kbd>

# Project Management
story;User Story;**As a** {{input:role}}\n**I want** {{input:goal}}\n**So that** {{input:benefit}}
ac;Acceptance Criteria;**Given** {{input:context}}\n**When** {{input:action}}\n**Then** {{input:outcome}}
bug;Bug Report;## Bug Report\n\n**Summary:** {{input:summary}}\n**Steps to Reproduce:**\n1. {{input:steps}}\n**Expected:** {{input:expected}}\n**Actual:** {{input:actual}}\n**Environment:** {{input:environment}}
spike;Spike Summary;## Spike: {{input:title}}\n\n**Objective:** {{input:objective}}\n**Findings:** {{input:findings}}\n**Recommendation:** {{input:recommendation}}\n**Time Spent:** {{input:hours}} hours
rfc;RFC / Proposal;## RFC: {{input:title}}\n\n**Author:** {{username}}\n**Date:** {{date}}\n\n**Problem:** {{input:problem}}\n**Proposal:** {{input:proposal}}\n**Alternatives Considered:** {{input:alternatives}}\n**Open Questions:** {{input:questions}}
blocker;Blocker Report;**Blocked:** {{input:task}}\n**Blocker:** {{input:reason}}\n**Impact:** {{input:impact}}\n**Needs:** {{input:action_needed}}
status;Status Update;## Status Update - {{date}}\n\n**Completed:**\n- {{input:done}}\n\n**In Progress:**\n- {{input:wip}}\n\n**Up Next:**\n- {{input:next}}\n\n**Risks:**\n- {{input:risks|None}}

# Documentation
readme;README Section;## {{input:section}}\n\n{{input:content}}
api;API Endpoint Doc;### {{input:method}} {{input:path}}\n\n**Description:** {{input:description}}\n\n**Request:**\n```json\n{{input:request_body}}\n```\n\n**Response:**\n```json\n{{input:response_body}}\n```
envdoc;Environment Variable Doc;| Variable | Description | Default | Required |\n|---|---|---|---|\n| `{{input:name}}` | {{input:description}} | {{input:default|-}} | {{input:required|Yes}} |
install;Installation Steps;## Installation\n\n```bash\n{{input:command}}\n```\n\nPrerequisites: {{input:prereqs}}
faq-entry;FAQ Entry;### {{input:question}}\n\n{{input:answer}}
arch;Architecture Note;## {{input:component}}\n\n**Purpose:** {{input:purpose}}\n**Dependencies:** {{input:deps}}\n**Key Files:** {{input:files}}

# SQL & Data
sel;SQL Select;SELECT {{input:columns|*}}\nFROM {{input:table}}\nWHERE {{input:condition}};
ins;SQL Insert;INSERT INTO {{input:table}} ({{input:columns}})\nVALUES ({{input:values}});
upd;SQL Update;UPDATE {{input:table}}\nSET {{input:column}} = {{input:value}}\nWHERE {{input:condition}};
del;SQL Delete;DELETE FROM {{input:table}}\nWHERE {{input:condition}};
cte;SQL CTE;WITH {{input:name}} AS (\n    {{clipboard}}\n)\nSELECT * FROM {{input:name}};
idx;Create Index;CREATE INDEX IX_{{input:table}}_{{input:column}}\nON {{input:table}} ({{input:column}});
migrate;Migration Script;-- Migration: {{input:description}}\n-- Date: {{date}}\n-- Author: {{username}}\n\nBEGIN TRANSACTION;\n\n{{input:sql}}\n\nCOMMIT;
connstr;Connection String;Server={{input:server}};Database={{input:database}};Trusted_Connection=True;TrustServerCertificate=True;

# HTML & Web
htmlpage;HTML Page;<!DOCTYPE html>\n<html lang="en">\n<head>\n    <meta charset="UTF-8">\n    <meta name="viewport" content="width=device-width, initial-scale=1.0">\n    <title>{{input:title}}</title>\n</head>\n<body>\n    {{clipboard}}\n</body>\n</html>
form;HTML Form;<form action="{{input:action}}" method="{{input:method|post}}">\n    <label for="{{input:id}}">{{input:label}}</label>\n    <input type="{{input:type|text}}" id="{{input:id}}" name="{{input:id}}" required>\n    <button type="submit">Submit</button>\n</form>
flexbox;Flexbox Container;display: flex;\njustify-content: {{input:justify|center}};\nalign-items: {{input:align|center}};\ngap: {{input:gap|1rem}};
grid;CSS Grid;display: grid;\ngrid-template-columns: {{input:columns|repeat(3, 1fr)}};\ngap: {{input:gap|1rem}};
media;Media Query;@media (max-width: {{input:breakpoint|768px}}) {\n    {{clipboard}}\n}
fetch;Fetch API Call;const response = await fetch('{{input:url}}', {\n    method: '{{input:method|GET}}',\n    headers: { 'Content-Type': 'application/json' },\n});\nconst data = await response.json();
axios;Axios Request;const { data } = await axios.{{input:method|get}}('{{input:url}}', {{clipboard}});

# Communication & Slack
update;Quick Update;Update: {{input:message}}\n\nContext: {{input:context}}
thanks;Team Thanks;Shoutout to {{input:name}} for {{input:achievement}}! Great work.
announce;Announcement;{{input:title}}\n\n{{input:details}}\n\nPlease reach out if you have questions.
eod;End of Day Update;EOD Update - {{date}}\n\nCompleted: {{input:done}}\nCarrying over: {{input:carry|Nothing}}
review-req;Review Request;Could someone review {{input:item}}? Context: {{input:context}}\n\nLink: {{input:link}}
oncall;On-Call Handoff;On-Call Handoff - {{date}}\n\n**Active Issues:** {{input:issues|None}}\n**Monitoring:** {{input:monitoring}}\n**Notes:** {{input:notes}}

# AI & Prompts
syspr;System Prompt;You are {{input:role}}. Your task is to {{input:task}}. Follow these guidelines:\n- {{input:guideline_1}}\n- {{input:guideline_2}}\n\nRespond in {{input:format|markdown}}.
rewrite;Rewrite Text;Rewrite the following text to be {{input:style|more concise and professional}}:\n\n{{clipboard}}
summarize;Summarize;Summarize the following in {{input:length|3 bullet points}}:\n\n{{clipboard}}
explain;Explain Code;Explain what this code does in plain language:\n\n{{clipboard}}
translate;Translate;Translate the following to {{input:language}}:\n\n{{clipboard}}
tone;Change Tone;Rewrite the following in a {{input:tone|friendly and professional}} tone:\n\n{{clipboard}}
proofread;Proofread;Proofread the following for grammar, spelling, and clarity. List any changes you make:\n\n{{clipboard}}
brainstorm;Brainstorm Ideas;Generate {{input:count|5}} ideas for {{input:topic}}. For each idea, provide a brief description and potential impact.
pros-cons;Pros and Cons;List the pros and cons of {{input:topic}}:\n\n**Pros:**\n-\n\n**Cons:**\n-
eli5;Explain Simply;Explain {{input:topic}} as if I were a beginner with no technical background. Use simple analogies.

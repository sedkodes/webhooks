```
## Final Result:



## JSON Payload:
{
	"blocks": [
		{
			"type": "section",
			"text": {
				"type": "plain_text",
				"emoji": true,
				"text": "New message from prospect:"
			}
		},
		{
			"type": "divider"
		},
		{
			"type": "section",
			"text": {
				"type": "mrkdwn",
				"text": "*From:* {{ticket.requester.name}}\n *Company:*{{ticket.organization.name}}\n*Subject:* {{ ticket.title }}"
			}
		},
		{
			"type": "divider"
		},
		{
			"type": "context",
			"elements": [
				{
					"type": "mrkdwn",
					"text": "*Assignee*: {{ticket.assignee.first_name}}\n*<https://{{ticket.url}}|View Ticket>*"
				}
			]
		}
	]
}
```

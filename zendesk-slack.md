## Final Result:


### Test on Slack
[Click Me][1]

## JSON Payload:
```
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

[1]: https://app.slack.com/block-kit-builder/T0ATUMNSJ#%7B%22blocks%22:%5B%7B%22type%22:%22section%22,%22text%22:%7B%22type%22:%22plain_text%22,%22emoji%22:true,%22text%22:%22New%20message%20from%20prospect:%22%7D%7D,%7B%22type%22:%22divider%22%7D,%7B%22type%22:%22section%22,%22text%22:%7B%22type%22:%22mrkdwn%22,%22text%22:%22*From:*%20Rob%20Smith%5Cn%20*Company:*%20Acme%20Org%5Cn*Subject:*%20%5C%22Trouble%20configuring%20SSL%5C%22%22%7D%7D,%7B%22type%22:%22divider%22%7D,%7B%22type%22:%22context%22,%22elements%22:%5B%7B%22type%22:%22mrkdwn%22,%22text%22:%22*Assignee*:%20Sedky%5Cn*%3Cfakelink.ToMoreTimes.com%7CView%20Ticket%3E*%22%7D%5D%7D%5D%7D

`{
    "comment": {
        "userId": "pgruenbaum",
        "discId": 964564445654,
        "time": "2022-09-27 10:04:32",
        "text": "Well said, Barb!!"
    }
}`

Note that the time is GMT and also optional. If not included, then it uses the current time when the request is received by the server

Represent a comment of a posting

| Element | Description | Type | Reuired| Notes |
| ---- | ---- | ---- | ---- | ---- |
| comment | Top Level | Comment data object | Required |  |
| &nbsp; &nbsp; userId | ID of user making comment | string | Required |  |
| &nbsp; &nbsp; discId | ID of the discussion is being commentd on | number | Required |  |
| &nbsp; &nbsp; time | time that the comment was posted | string | Optional | YYYY-MM-DD HH:MM:SS Greenwich Mean Time. Default is the time the comment is received by the server |
| &nbsp; &nbsp; text | text of the comment | string | Required |  |

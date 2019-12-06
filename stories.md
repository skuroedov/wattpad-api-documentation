# Stories

---

You can list stories containing some tag, string in title, description, etc.:

`https://api.wattpad.com/v4/stories?query=<string>`

Or get story using id:

`https://api.wattpad.com/v4/stories?query=<id>`

Result:

```
{
    "stories": [
	{
	    "id": int,
	    "title": string,
	    "length": int,
	    "createDate": string(date),
	    "modifyDate": string(date),
	    "voteCount": int,
	    "readCount": int,
	    "commentCount": int,
	    "language": {
		"id": int,
		"name": string
	    },
	    "user": {
		"name": string,
		"avatar": string(url),
		"fullname": string
	    },
	    "description": string,
	    "cover": string(url),
	    "cover_timestamp": string(date),
	    "completed": boolean,
	    "categories": [
		int,
		...
	    ],
	    "tags": [
		string,
		...
	    ],
	    "rating": int,
	    "mature": boolean,
	    "copyright": int?,
	    "url": string(url),
	    "firstPartId": int,
	    "numParts": int,
	    "firstPublishedPart": {
		"id": int,
		"createDate": string(date)
	    },
	    "lastPublishedPart": {
		"id": int,
		"createDate": string(date)
	    },
	    "parts": [
		{
		    "id": int,
		    "title": string,
		    "url": string(url),
		    "rating": int,
		    "draft": boolean,
		    "modifyDate": string(date),
		    "createDate": string(date),
		    "length": int,
		    "videoId": int,
		    "photoUrl": string(url),
		    "commentCount": int,
		    "voteCount": 162,
		    "readCount": int
		},
		...
	    ],
	    "deleted": boolean
	},
	...
    ],
    "total": int,
    "nextUrl" string(url)
}
```


<!-- Simple code documentation -->
`<recordTV>
 <date>2015-06-01</date>
 <time format="24">18:00</time>
 <duration>1.5</duration>
 <channel>54</channel>
</recordTV>`

Represents a request to record a television program

| Element | Description | Type | Requested | Notes |
| ---- | ---- | ---- | ---- | ---- |
| recordTV | Top level | TV program data | required |  |
| &nbsp; &nbsp;date | Date of the program | string | optional | Format is YYYY-MM-DD HH:MM:SS. Default value is today's date|
| &nbsp; &nbsp;time | Time the program begins | string | required | Att.: **format** has values `24` or `12` for 24 or 12 hour formats. Format is HH:MM, with am or pm afterwords for 12 hour format |
| &nbsp; &nbsp;duration | Length of the program | number | required | In hours |
| &nbsp; &nbsp;channel | Channel to record | number | required |  |


<!-- Atribute code documentation -->
<recordTV>
 <when date="2015-06-01" time="18:00" format="24"/>
 <duration hours="1.5"/>
 <station channel="54"/>
</recordTV>

Represents a request to record a television program


| Element | Attribute | Description | Type | Requested | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| recordTV |  | Top level | TV program data | required |  |
| &nbsp; &nbsp;when |  | Date and time the program start | TV program data | required |  |
|  | date | Date  | string | optional | Format is YYYY-MM-DD. Default value is today's date|
|  | time | Time the program begins | string | required | Format is HH:MM, with am or pm afterwords for 12 hour format |
|  | format | format of the time: either 12 hours or 24 hours | string | required | Valid values: `24` or `12` |
| &nbsp; &nbsp;duration | hours | Length of the program | number | required | In hours |
| &nbsp; &nbsp;station | channel | Channel to record | number | required |  |


<!-- Complex code Documentation -->
<dailyData>
 <date>2015-06-01</date>
 <hourlyData>
 <time>10:00</time>
 <device>
 <id>34</id>
 <temperature>70</temperature>
 <humidity>11</humidity>
 </device>
 <device>
 <id>35</id>
 <temperature>72</temperature>
 <humidity>12</humidity>
 </device>
 ...
 </hourlyData>
 <hourlyData>
 <time>11:00</time>
 <device>
 <id>34</id>
 <temperature>71</temperature>
 <humidity>10</humidity>
 </device>
 ...
 </hourlyData>
 ...
</dailyData>


Pending
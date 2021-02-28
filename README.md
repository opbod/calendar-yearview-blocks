# calendar-yearview-blocks
jQuery plugin for showing a calendar yearview with blocks (github contributions style)

Code adopted from https://github.com/bachvtuan/Github-Contribution-Graph and expanded.

Allows for up to 4 items per day that will be shown on the calendar (square, triangle, stripes and cubes, respectively).
Expects a JSON as data input in the form of:

    {
        "2020-08-01": {
            "items": ["banana", "apple"]
        }, 
        "2020-09-01": {
            "items": ["orange"]
        }
    }

Settings are self-explanatory:

    $('#cal_chart_1').calendar_yearview_blocks({
        data: '{"2020-08-01": {"items": ["banana", "apple"]}, "2020-05-05": {"items": ["apple"]}, "2020-05-01": {"items": ["banana"]}, "2020-05-03": {"items": ["banana", "apple", "orange"]}, "2020-05-22": {"items": ["banana", "apple", "orange", "pear"], "legend": "The whole basket"}}',
        start_monday: true,
        always_show_tooltip: true,
		stylize_today: false, // Draw a box around today's date.
		//final_date: '2021-12-31', // Set the last date to be displayed. If not set, defaults to the current day.
		tooltip_style: 'default', // 'default': the tooltip will include the date, newline, and the values.
                                 // The values can be overridden by including a 'legend' value in the data object.
                                 // 'custom': the 'legend' value will encompass the entire tooltip.
        month_names: ['jan', 'feb', 'maa', 'apr', 'mei', 'jun', 'jul', 'aug', 'sept', 'okt', 'nov', 'dec'],
        day_names: ['ma', 'wo', 'vr', 'zo'],
        colors: {
            'default': '#eeeeee', // Default color
            'apple': 'green',
            'banana': 'yellow',
            'orange': 'orange',
            'pear': 'lightgreen'
        }
    });

![Demo screenshot](https://i.ibb.co/SNPVw2q/calendar-yearview-blocks.jpg "Demo screenshot")

MIT license

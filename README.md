# calendar-yearview-blocks
jQuery plugin for showing a calendar yearview with blocks (github contributions style)

Code adopted from https://github.com/bachvtuan/Github-Contribution-Graph and expanded.

Allows for up to 4 items per day that will be shown on the calendar (square, triangle, stripes and cubes, respectively).
Settings are self-explanatory:

    $('#cal_chart_1').calendar_yearview_blocks({
        data: '{"2020-08-01": {"items": ["banana", "apple"]}, "2020-05-05": {"items": ["apple"]}, "2020-05-01": {"items": ["banana"]}, "2020-05-03": {"items": ["banana", "apple", "orange"]}, "2020-05-22": {"items": ["banana", "apple", "orange", "pear"]}}',
        start_monday: true,
        always_show_tooltip: true,
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

![Demo screenshot](https://i.ibb.co/Dgssfc6/calendar-yearview-blocks.jpg "Demo screenshot")

<div align="center">
    <img src="https://github.com/frappe/design/blob/master/logos/logo-2019/frappe-gantt-logo.png" height="128">
    <h2>Frappe Gantt - Jalali </h2>
    <p align="center">
        <p>A simple, interactive, modern jalali gantt chart library for the web</p>
        <a href="https://gantt.yiiman.ir/">
            <b>View the jalali demo »</b>
        </a>
    </p>
</div>

<p align="center">
    <a href="https://frappe.github.io/gantt">
        <img src="https://github.com/yiiman-dev/gantt/blob/master/.images/jalali.png">
    </a>
</p>

### Install
```
npm install frappe-gantt-jalali
```

### Usage
Include it in your HTML:
```
<script src="dist/frappe-gantt.min.js"></script>
<link rel="stylesheet" href="dist/frappe-gantt.css">
```

And start hacking:
```js
var tasks = [
  {
    id: 'Task 1',
    name: 'Redesign website',
    start: '2016-12-28',
    end: '2016-12-31',
    progress: 20,
    dependencies: 'Task 2, Task 3',
    custom_class: 'bar-milestone' // optional
  },
  ...
]
var gantt = new Gantt("#gantt", tasks);
```

You can also pass various options to the Gantt constructor:
```js
var gantt = new Gantt("#gantt", tasks, {
    header_height: 50,
    column_width: 30,
    step: 24,
    view_modes: ['Quarter Day', 'Half Day', 'Day', 'Week', 'Month'],
    bar_height: 20,
    bar_corner_radius: 3,
    arrow_curve: 5,
    padding: 18,
    view_mode: 'Day',   
    date_format: 'YYYY-MM-DD',
    custom_popup_html: null,
    is_jalali: true,
    language: 'fa'
});
```

If you want to contribute:

1. Clone this repo.
2. `cd` into project directory
3. `yarn`
4. `yarn run dev`

License: MIT

------------------
Project maintained by [frappe](https://github.com/frappe)

and converted to jalali by [YiiMan](https://github.com/yiiman-dev)


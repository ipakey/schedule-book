class structure for calendar

Left

````<div class="left">
    <div class="calendar">
        <div class="month">
        <div class="arrow prev"></div>
        <div class="date"></div>
        <div class="arrow next"></div>
        </div>
        <div class="weekdays">
            <div class="dayName"></div>
        </div>
        <div class="days">
            <!-- ! days will be added with js -->
        </div>
        <div class="goto-today">
            <div class="goto event-btn">
                <input type="text" name="" id="" class="date-input">
                <button class="event-btn"> </button>
            </div>
            <div class="today-btn"></div>
        </div>
    </div>
</div>```
````

Right:

````<div class="right">
    <div class="today-date">
        <div class="event-day"></div>
        <div class="event-date"></div>
    </div>
    <div class="events">
        <!-- todo events to be added by js -->
    </div>
    <div class="add-event-wrapper">
        <div class="add-event-header">
            <div class="title"></div>
            <img src="" alt="" class="arrow">
        </div>
        <div class="add-event-body">
            <div class="add-event-input">
                <input type="text" name="" id="event-name" class="event-name" placeholder="" required>
            </div>
            <div class="halfway">
                <div class="add-event-input">
                    <label for="time-input-from">  </label>
                    <input type="text" name="" id="time-input-from" class="event-time">
                    <span class="validity"></span>
                </div>
                    <div class="add-event-input"></div>
                    <label for="time-input-to">  </label>
                    <input type="text" name="" id="time-input-to" class="event-time">
                    <span class="validity"></span>
                </div>
            </div>
            <div class="add-event-input">
                <input type="text" name="" id="event-details" class="event-details" placeholder="">
            </div>
        </div>

        <div class="add-event-footer">
            <button type="submit" class="add-event-btn event-btn add-btn"></button>
            <button type="submit" class="edit-event-btn event-btn edit-btn"></button>
            <button type="submit" class="close-event-btn event-btn close-btn"></button>
        </div>
        <div class="menu-buttons">
            <button class="manage-events-btn event-btn"></button>
        </div>


    </div>
</div>
</div>```
````

---

script structure

1. variable declaration
1. initialise data
1. default array = sqli process
1. function initCalendar() {}
1. initCalendar()

<!-- ! run process  -->
<!-- ! button functiality-->

function prevMonth(){}
function nextMonth(){}

1. add eventListener

- prev,
- next,
- goto,
- today,
- dateInput,
- gotoDate

<!-- ! button functionality  -->

1. add eventListeners

- addEventBtn,
- addEventCloseBtn
- close from outside form

<!-- ! Event Validation  -->

1. add eventListeners for addEventTo & addEventFrom

- 50chars in field
- time format
- remove char not number
- add leading 0
- no more than 5 char total

1. function addListener(){

- define variables
- set current day as active day
- call active day after click
- remove active from previous active day
- if prev month clicked go to prev month and add active
- select all days of that month
- add active to clicked day
  }

function getActiveDate(date){ - define variable day & dayName

- .innerHtml dayName
- .innerHtml date + month +year
  }

<!-- ! Show events of the day -->

function updateEvents(date){
define events
access eventsArr forEach((event) =>{
get events for active day only
`if (all parts of date match active day)`
show event on document with inserted HTML

            ```
            events += `
            <div class="event">
                <div class="title">
                    <img class="list-icon " src="./images/cogs.png" alt="" srcset="">
                    <h3 class="event-title">${event.title}
                    <h3 class="event-time">${event.from} - ${event.to}</h3>
                </div>
                <div class="event-details">
                    <p>${event.details}</p>
                </div>
            </div>`
                ```
        `if(null)`
            ```events = ` <div class="no-event">
                    <p>No Events</p></div>`
            ```

    eventsContainer.innerHTML = events
    })

}

<!-- ! Add an Event listener-->

addEventSubmit{ - define variables from input form - validate data - all fields full - time format correct - add new event to array
}

<!-- todo write record to database -->

reset active form fields to blank

update the current day records updateEvents(activeDay)

function convertTime(time){ - split and format time into 12 hr format - return time
}

<!-- todo date and year picker -->

function (){}
function (){}

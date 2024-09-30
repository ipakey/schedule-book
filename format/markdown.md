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
            <!-- todo days will be added with js -->
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

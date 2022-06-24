
Use case:
- User1 gets email from User2 wanting to book a meeting
- User1 sends back a link to a site 
- User2 opens site and sees a UI with available time slots
- User2 picks presses a time slot and creates a booking
- User1 gets notified about the requested booking
- User1 can approve or disapprove the booking

Requirements:
- Should be able to add events in google calendar
- Should be able to send email notifications
- Should be able to show available spots
- Should check user calendar in case they book something into available spots
- User should be able to pick which times are going to be available to book, weekly, monthly or yearly (for instance Tuesdays at 3PM is available all year, Monday at 2PM is only available today etc)
- User that books meeting should be able to add in details for the meeting
    - Might have options like: type of meeting [Phone, Video, Face to Face]
    - Adding in a note for what the meeting is about 
    - Name of booker, name of company
    - Phone number and email
    - if it's a video conference an option for adding a link to the site of the meeting is required
- Main user should be able to approve or disapprove booking 

Edge cases:
- User1 is in the process of booking appointment and User2 books it before User1 finishes. So once User1 is done it is no longer available.
    - Solution: When a user presses a time slot it becomes unavailable straight away. And if they cancel or get disapproved it will become available again.
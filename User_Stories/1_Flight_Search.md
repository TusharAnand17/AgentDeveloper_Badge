US1.1 – Search for a One-Way Flight
As a traveler, I want to search for a one-way flight by selecting departure city, destination city,
departure date, number of passengers, and travel class so that I can view available flight options for
a single journey.
Acceptance Criteria:
• From (Departure City): Dropdown with cities (New York, London, Tokyo, Paris, Sydney,
Mumbai, Delhi, Dubai, Singapore). Default = 'Select City'. Mandatory. Error if blank →
'Please select a departure city.'
• To (Destination City): Same as From. Mandatory. Error if blank → 'Please select a
destination city.' If same as 'From' → 'Departure and destination cannot be the same.'
• Departure Date: Calendar picker (month navigation, today highlight, clear). Manual entry in
dd-mm-yyyy allowed. Past dates disabled. Mandatory. Error if blank → 'Please select a
departure date.'
• Return Date: Hidden when 'One Way' is checked.
• Passengers: Numeric input (1–9) with arrows. Default = 1. Error if invalid → 'Please enter
between 1 and 9 passengers.' Not mandatory, defaults to 1.
• Travel Class: Dropdown with Economy (default), Business, First. Not mandatory, defaults
to Economy.
• One Way Checkbox: Unchecked by default. Checked → hides Return Date. Unchecked →
Return Date reappears.
• Search Button: Disabled until all mandatory fields valid. On click, validate inputs. Errors
highlighted below fields. If valid → show results page.
• Results: List of available departure flights with airline, flight number, cities, dates/times,
duration, price (USD). Sorted by departure time. If none → 'No flights available for selected
criteria.'
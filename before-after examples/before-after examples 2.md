Example 2: Logging to a File

Initial Prompt

How do I log the temperature to a file after getting it from the weather API?

Initial AI-Generated Code (Before)

log = open("log.txt", "a")
log.write("Temp data")
log.close()

My Analysis

Not integrated with actual temperature data

Not using context manager

No formatting or timestamp

Follow-up Prompt

Update this so it logs the real temperature with condition and timestamp using a with block.

Improved Code (After)

import datetime

with open("log.txt", "a") as log:
    timestamp = datetime.datetime.now().isoformat()
    log.write(f"{timestamp} - {city}: {temp}°C, {condition}\n")

Why the Prompt Worked

Targeted a specific weak point (poor logging practice)

Asked for useful features (real data, timestamp, file safety)

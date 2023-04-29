# Time-table
F22BSEEN1E02113 

# Create a list of weekdays and class times
days = ['Saturday', 'Sunday', 'Monday', 'Tuesday', 'Wednesday', 'Thursday']
times = ['8:30 AM - 10:00 AM', '10:15 AM - 11:45 AM', '12:00 PM - 1:30 PM', 
         '2:00 PM - 3:30 PM', '3:45 PM - 5:15 PM', '5:30 PM - 7:00 PM']

# Create a dictionary of courses and their timings
timetable = {
    'Saturday': {
        '8:30 AM - 10:00 AM': 'CSE1101 Lecture (Section 1)',
        '10:15 AM - 11:45 AM': 'CSE1101 Lab (Section 1)',
        '12:00 PM - 1:30 PM': 'CSE1101 Lecture (Section 2)',
        '2:00 PM - 3:30 PM': 'CSE1101 Lab (Section 2)',
    },
    'Sunday': {
        '8:30 AM - 10:00 AM': 'CSE1103 Lecture',
        '10:15 AM - 11:45 AM': 'CSE1103 Lab',
        '2:00 PM - 3:30 PM': 'CSE1107 Lecture',
        '3:45 PM - 5:15 PM': 'CSE1107 Lab',
    },
    'Monday': {
        '8:30 AM - 10:00 AM': 'CSE1102 Lecture',
        '10:15 AM - 11:45 AM': 'CSE1102 Lab',
        '12:00 PM - 1:30 PM': 'CSE1104 Lecture',
        '2:00 PM - 3:30 PM': 'CSE1104 Lab',
    },
    'Tuesday': {
        '8:30 AM - 10:00 AM': 'CSE1105 Lecture',
        '10:15 AM - 11:45 AM': 'CSE1105 Lab',
        '2:00 PM - 3:30 PM': 'CSE1109 Lecture',
        '3:45 PM - 5:15 PM': 'CSE1109 Lab',
    },
    'Wednesday': {
        '8:30 AM - 10:00 AM': 'CSE1106 Lecture',
        '10:15 AM - 11:45 AM': 'CSE1106 Lab',
        '12:00 PM - 1:30 PM': 'CSE1110 Lecture',
        '2:00 PM - 3:30 PM': 'CSE1110 Lab',
    },
    'Thursday': {
        '8:30 AM - 10:00 AM': 'CSE1108 Lecture',
        '10:15 AM - 11:45 AM': 'CSE1108 Lab',
        '2:00 PM - 3:30 PM': 'CSE1112 Lecture',
        '3:45 PM - 5:15 PM': 'CSE1112 Lab',
        '5:30 PM - 7:00 PM': 'CSE1114 Lecture',
    }
}

# Print the timetable
print('IUB CSE Department Time Table')
print('----------------------------')
for day in days:
    print(day)
    print('----------------------------')
    for time in times:
        if time in timetable[day]:
            print(time, timetable[day][time].

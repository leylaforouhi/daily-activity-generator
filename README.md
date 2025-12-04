import datetimE
import os

def update_log_file():
    now = datetime.datetime.now()
    message = f"Last update: {now.strftime('%Y-%m-%d %H:%M:%S')}"

    with open("activity_log.txt", "a") as file:
        file.write(message + "\n")

    print("Activity updated successfully!")

if __name__ == "__main__":
    update_log_file()


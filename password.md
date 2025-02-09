import time
import sys

attempts = 3
while attempts > 0:
    text = input("ENTER PASSWORD: ").strip()


    if text == "1801999":
        print("HI BRO!")
        break
    else:
        attempts -= 1
        if attempts > 0:
            print(f"Incorrect password! {attempts} attempts left.")
        else:    
            print("Access denied!")
            time.sleep(1)
            
            def countdown_timer(seconds):
                for sec in range(seconds, 0, -1):
                    sys.stdout.write(f"{sec:02} seconds remaining...\r")
                    sys.stdout.flush()
                    time.sleep(1)
                print("\n")
            countdown_timer(3)
            
            messages = ["\n*** I N F O  D E L E T E D ***", "\n*** G O O D  B Y E ***", "\n\t   😉"]
            for message in messages:
                time.sleep(1)
                print(message)

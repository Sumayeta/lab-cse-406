# lab-cse-406
class processes:
    def __init__(self, id, at, bt, ct):
        self.id = id
        self.at = at
        self.bt = bt
        self.ct = ct
        self.tat = self.ct-self.at
        self.wt = self.tat-self.bt


num = int(input("Enter the Number of Processes:"))
l = []
ct = 0

for i in range(num):

avg_tat = 0
avg_wat = 0
print("PID\tAT\tBT\tCT\tTAT\tWT")
for process in l:
    process.get()

for process in l:
    avg_wat += process.waiting()
print(f"Avg_Waitingtime:{avg_wat/num}")

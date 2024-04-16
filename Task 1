class Task:
    def init(self, name, priority, due_date, completed=False):
        self.name = name
        self.priority = priority
        self.due_date = due_date
        self.completed = completed
    
    def str(self):
        status = "Completed" if self.completed else "Not Completed"
        return f"Task: {self.name}, Priority: {self.priority}, Due Date: {self.due_date}, Status: {status}"
class TaskManager:
    def init(self):
        self.tasks = []

    def add_task(self, task):
        self.tasks.append(task)

    def remove_task(self, task_name):
        self.tasks = [task for task in self.tasks if task.name != task_name]

    def mark_task_completed(self, task_name):
        for task in self.tasks:
            if task.name == task_name:
                task.completed = True
                break

    def display_tasks(self):
        if not self.tasks:
            print("No tasks found.")
        else:
            for task in self.tasks:
                print(task)

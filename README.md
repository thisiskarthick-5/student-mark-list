# student-mark-list

    class student:
      def __init__(self,name,roll,marks):
          self.name = name
          self.roll = roll
          self.marks = marks
          
      def total_marks(self):
          return sum(self.marks)  
      
      def average_mark(self):
          return sum(self.marks)/len(self.marks) if self.marks else 0
      
      def display_info(self):
          mark_str = ",".join(str( (mark) for mark in self.marks))
          return(f"STUDENT NAME : {self.name.upper()} \n"
                 f"STUDENT ROLLNO : {self.roll} \n"
                 f"STUDENT MARKS : {self.total_marks()} \n"
                 f"AVERAGE MARK : {self.average_mark()} \n")
          
          
    student1 = student("karthick","202",[98,87,76,67,98])
    print(student1.display_info()) 
           
                 
      
          
          
          
          

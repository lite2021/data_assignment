# data_assignment

#define lists for each attributes
list_Price = []
list_Maintenance_cost = []
list_Number_of_doors = []
list_Number_of_passengers = []
list_Luggage_capacity = []
list_Safety_rating = []
list_Classification_of_vehicle = []
#import library csv
import csv
with open('C:/Users/89807/OneDrive/Desktop/Python_1/3 week/cars-sample35.txt') as csvfile:
 readCSV = csv.reader(csvfile) #read data
# print each row value as list by using the csv.reader function
 for row in readCSV:
    
    list_Price.append(row[0]) #extract index=0 values from each row list in readCSV to become the list of price 
    list_Maintenance_cost.append(row[1]) 
    list_Number_of_doors.append(row[2])
    list_Number_of_passengers.append(row[3])  
    list_Luggage_capacity.append(row[4])
    list_Safety_rating.append(row[5])
    list_Classification_of_vehicle.append(row[6])
print("Price:", list_Price)
print("Maintenance_cost:", list_Maintenance_cost)
print("Number_of_doors:", list_Number_of_doors)
print("Number_of_passengers:", list_Number_of_passengers)
print("Luggage_capacity:", list_Luggage_capacity)
print("Safety_rating:", list_Safety_rating)
print("list_Classification_of_vehicle:", list_Classification_of_vehicle)

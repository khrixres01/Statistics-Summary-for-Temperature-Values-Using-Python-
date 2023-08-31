# Statistics-Summary-for-Temperature-Values-Using-Python-

#Finding the data summary of different temp. ranges

#import statistics to make life easier
import statistics

#temperature values 
Temp_val = [36.5,36.8,38.5,37.8,35.7,39.2,36.9,35.1,39.2,35.7,39.2,36.9,35.1,39.2,39.2,35.7,39.2,36.9,35.1,39.2,]

#sorted list of temperature values
sorted_temp = sorted(Temp_val)

#mean of temperature values
mean_temp = statistics.mean(sorted_temp)

#median grouped values
median_temp = statistics.median_grouped(sorted_temp)

#mode of temperature values
mode_temp = statistics.mode(sorted_temp)

#range between temperature values
range_temp = (max(sorted_temp) - min(sorted_temp))

#standard deviation of the temperature values
standard_dev = statistics.stdev(sorted_temp)

#variance of the temperature values
variance = statistics.variance(sorted_temp,mean_temp)

#mean deviation of the temperature values
mean_deviation = sum(abs(x - mean_temp) for x in Temp_val) / len(Temp_val)


print(f'mean value: {mean_temp:.2f}')
print(f'median value: {median_temp:.2f}')
print(f'mode value: {mode_temp:.2f}')
print(f'range value: {range_temp:.2f}')
print(f'mean_deviation: {mean_deviation:.2f}')
print(f'standard_deviation: {standard_dev:.2f}')
print(f'variance_value: {variance:.2f}')


![stat summaryy](https://github.com/khrixres01/Statistics-Summary-for-Temperature-Values-Using-Python-/assets/105367501/847694c1-a114-45db-adc2-a1d6249e3238)

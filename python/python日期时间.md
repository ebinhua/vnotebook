# python_datetime


from datetime import datetime, date, timedelta

get the date：
yesterday = date.today() + timedelta(days = -1)  

格式化输出
yesterday = (date.today() + timedelta(days = -1)).strftime("%Y-%m-%d")

星期
import calendar

calender.MONDAY
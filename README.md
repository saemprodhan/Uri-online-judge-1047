# Uri-online-judge-1047
Game Time with Minutes
start_hour, start_minute, end_hour, end_minute = map(int, input().split())
total_start = (start_hour * 60) + start_minute
total_end = (end_hour * 60) + end_minute
if total_end > total_start:
    duration = total_end - total_start
else:
    duration = (24 * 60 - total_start) + total_end
duration_hour = duration // 60
duration_minute = duration % 60
print(f"O JOGO DUROU {duration_hour} HORA(S) E {duration_minute} MINUTO(S)")

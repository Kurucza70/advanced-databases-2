A megoldandó feladatok szövegét is bemásolom ide.

2. Listázd ki a részlegek nevét (`DEPARTMENT_NAME`) a `DEPARTMENTS` táblából, ábécésorrendbe rendezve!

SELECT department_name
FROM hr.departments
ORDER BY department_name ASC;

3. Keresd meg azokat a munkaköröket a `JOBS` táblában, ahol a maximális fizetés (`MAX_SALARY`) meghaladja a 10 000-et!

SELECT *
FROM hr.jobs
WHERE max_salary > 10000;

5. Listázd ki a `LOCATIONS` táblából a városokat (`CITY`) és az államokat/tartományokat (`STATE_PROVINCE`), de csak azokat a sorokat, ahol a tartomány ki van töltve!

SELECT city, state_province
FROM hr.locations
WHERE state_province IS NOT NULL;


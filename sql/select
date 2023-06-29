SELECT COUNT(S.id) AS quantity, city_id, C.name FROM scooter AS S
INNER JOIN cities AS C ON S.city_id = C.id
GROUP BY S.city_id;

SELECT U.id , CONCAT( first_name, " ", last_name) AS name, C.name AS city,P.name AS province,K.name AS country
FROM users AS U
INNER JOIN address AS A ON U.id = A.user_id
INNER JOIN cities AS C ON A.city_id = C.id
INNER JOIN provinces AS P ON  P.id = C.province
INNER JOIN countries AS K ON k.id = P.country;

SELECT delivered_item_id,delivered_location_id FROM return_and_upkeep WHERE item_condition = "irreparable";

SELECT U.id, U.first_name, U.last_name, S.id, S.name, R.contract_start_date, R.contract_end_date
FROM rent_detail AS R
INNER JOIN users AS U ON U.id = R.customer_id
INNER JOIN scooter AS S ON S.id = R.rented_item_id
WHERE contract_start_date BETWEEN "2023-03-20" AND "2023-06-20";

SELECT U.id, U.first_name, U.last_name, S.id, S.name, R.contract_start_date, R.contract_end_date
FROM rent_detail AS R
INNER JOIN users AS U ON U.id = R.customer_id
INNER JOIN scooter AS S ON S.id = R.rented_item_id
GROUP BY R.customer_id
HAVING COUNT(R.customer_id) > 5 AND contract_start_date BETWEEN "2023-02-20" AND "2023-07-20";
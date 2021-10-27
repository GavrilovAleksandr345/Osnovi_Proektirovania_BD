USE store;
SELECT category.name AS category_name , good.name AS good_name FROM category_has_good as chg
INNER JOIN good
ON good.id = chg.good_id
INNER JOIN category
ON category.id = chg.category_id
ORDER BY good_name

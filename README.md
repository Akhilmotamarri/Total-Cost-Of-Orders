# Total-Cost-Of-Orders
Total Cost Of Orders
select cust_id,first_name,SUM(total_order_cost) from customers
join orders  ON customers.id=cust_id
group by cust_id,first_name
order by first_name
;

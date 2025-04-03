# Player-Signup-and-Deposit-Analysis
Player Signup and Deposit Analysis - IGaming

The attached dataset contains information for players that signed up between July and September, from a small group of Countries.

You'll find a unique identifier for each player, the signup date, Country, currency and the dates of their deposit with the status of the deposit and the amount deposited. The date of the deposit is formatted as "days from signup" (for example when the value is 3,it means that the player deposited 3 days after completing registration).

Could you please prepare a small presentation for the Acquisition Manager on :
- Signups trend
- FTDs trend
- New registrations deposits behaviour

If you would have to recreate this dataset starting from the following tables, how would you do it? (in SQL)

Table 1 has the following columns:
account_id: varchar
userID: varchar
userName: varchar
first_name: varchar
last_name: varchar
test_account: bool
country_id: varchar
brand_id: varchar
date_created: varchar
status_id: varchar

Table 2:
deposit_id: int
deposit_started_date: varchar
deposit_account_id: float
deposit_updated_date: varchar
deposit_payment_method_id: int
deposit_amount: varchar
deposit_amount_eur: float
deposit_status: varchar
deposit_currency_id: varchar
deposit_currency: varchar
deposit_reversed: bool

Table 3:
currency_id: varchar
currency_from: varchar
currency_to: varchar
currency_exchange_rate: float
Table 4:
 account_id: int
 status_id: int
 user_locked: bool

Extra questions:
Please provide a distribution of the deposits, including the 5th and 95th percentiles.
Lets suppose we need to run this distribution but per country in order to spot any trend difference.
How would you provide these distributions in a table, by countries (row) in an automated way?
Please include the cumulative successful and total deposits sums, per userID.

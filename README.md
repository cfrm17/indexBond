# Pricing Index Linked Bond


An index linked bond is one whose cash flows are linked to movements in a specific price index, with the aim of providing investors with a means to protect the real value of their savings. The bonds are usually indexed to a broad measure of prices, typically a domestic Consumer Price Index (CPI). 

 Index linked bonds include Canadian Real Return Bonds, US Treasury Inflation Indexed Securities (TIPS), OAT€i bonds and inflation GILTs. 

The index calculations for all target bonds are based on CPI for the currency of issue.  The index ratio for a given settlement date,  , is defined as the ratio of the reference CPI applicable to the settlement date divided by the reference CPI applicable to the original issue date of the bond:

 ,					        (1)

The reference CPI for the first day of any calendar month is the CPI for the calendar month falling three months earlier. For example, the reference CPI for 1 June corresponds to the CPI for March. Since CPI is set at the first day of each month, the reference CPI for settlement or issue dates not falling on the first day of the months are linearly interpolated according to the formula:

 ,		        (2)

where, 
D = The number of days in the calendar month in which the settlement date occurs.
d = The day of the month of the settlement date.
 = The reference CPI for the first day of the month in which the settlement date falls.
 = The reference CPI for the first day of the calendar month immediately following the settlement date.

For example, the reference CPI for 20 July, 1996 is calculated as follows:

 ,

                   

where D=31 and d=20. The value  is calculated in an identical fashion.  

The PV01, duration, and convexity for an index-linked bond are calculated by using the following relationships:

 					(3)
 					(4)

where,
t = settlement date
  = price of an index linked bond at t as a function of the real yield y.
  = price of a real bond at t with real yield that has the same maturity and coupon payment schedule as the index linked bond;
y = real yield of the bond (see https://finpricing.com/lib/FiZeroBond.html);
n = nominal yield of the bond;
 = assumed inflation rate;
f = coupon frequency.


The annual inflation rate   is calculated as:

 .					(5)

  is market observable and the index ratio,  , is calculated as in equation (1). Then, the real yield of the bond can be calculated using the relation in (3). Let this calculated real yield as y*. Without any confusion, the settlement date t is omitted from the formulae hereinafter.

Risk number calculations (PV01, modified duration and convexity) are given by:

 ,		(6)
 ,		(7)

 .			(8)


where,
   = PV01 of the index linked bond.
  = PV01 of a real bond with real yield that has the same maturity and coupon payment schedule as the index linked bond;
 	= convexity of the index linked bond;
 	= convexity of a real bond with real yield that has the same maturity and coupon payment schedule as the index linked bond;

Here,  represents the degree with which a move in inflation rates corresponds to a move in nominal rates.  


# SmartPark — Working Prototype v4

## Updated fixes
- Fresh launch always opens the SmartPark sign-in screen; a previous browser session does not bypass login.
- Account-specific bookings remain isolated by signed-in user.
- My Bookings shows current/upcoming bookings with booking IDs and QR actions, plus clearly labeled previous-trip history.
- Entry & Exit shows the selected booking ID and lets the signed-in user scan their own QR without manually typing the ID.
- Vehicle number is checked against the selected account booking.
- Inside Parking navigation uses a clear top-down floor layout with labeled bays, drive lane, entry gate, route, vehicle position and highlighted assigned bay.
- The highlighted bay updates dynamically to the user's assigned slot.

## Demo accounts
- User: jiya@smartpark.demo / 123456
- User: ananya@smartpark.demo / 123456
- Admin: admin@smartpark.demo / admin123

## Demo flow
1. Open index.html — login appears immediately.
2. Sign in as Jiya.
3. Find Parking → Search Parking → select a free slot → Continue to payment.
4. Choose UPI/Card/Net Banking/Wallet → Pay & Generate QR.
5. The booking confirmation shows the Booking ID and QR ticket.
6. Open Entry & Exit → select the booking → Scan QR.
7. The vehicle is verified and the barrier opens.
8. Follow the top-down navigation map to the highlighted slot.
9. Process Exit to release the slot.
10. Logout and sign in as Ananya to confirm account isolation.

This is a frontend-only hackathon prototype. Browser localStorage is used for demo persistence; production authentication, database authorization, payment gateway, QR scanner hardware and ANPR would be backend/infrastructure integrations.

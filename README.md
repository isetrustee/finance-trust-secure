# ISET Fiduciary Finance App

A comprehensive trust-based FinTech platform built with React Native and Expo, aligned with BIS mBridge, ISO 20022, and Open Finance principles.

## Features

### Authentication & Security
- 6-digit PIN entry system
- OTP verification
- Biometric authentication support
- Multi-factor authentication ready
- KYC/CDD verification flow

### Fiduciary Management
- Total liquid assets dashboard
- 10+ financial categories (Rewards, Incentives, Subsidies, Allocations, Gifts, Endowments, Investment Pool, Vouchers, Goals)
- Transaction history with detailed breakdowns
- Real-time balance updates

### Payment & Subscription System
- Send/Receive payments
- Multiple transfer methods (SWIFT, IBAN, ACH, RTGS, RippleNet, Local)
- Linked bank account management
- QR code payment support
- Bills and recurring subscriptions
- Payment facilitation (non-custodial)

### Community & Social
- Community projects dashboard
- 7 mission-focused tabs (Family, Projects, Communication, Development, Initiatives, Tourism, Environment, Agriculture)
- Social feed with posts and interactions
- Real-time project progress tracking
- Ecotourism showcase

### Account Management
- Household accounting
- Multiple linked bank accounts
- Payables, loans, and subscriptions tracking
- Profile management with tier system (Basic → Skilled → Advanced → Expert → Official)
- Trust instrument viewer

### Messaging
- Inbox/Sent/Announcements tabs
- Real-time notifications
- Transaction receipts and vouchers

### Admin Features
- Admin dashboard with key metrics
- User activity monitoring
- System-wide statistics
- Content management capabilities

## Tech Stack

- **Framework**: React Native with Expo
- **Navigation**: Expo Router
- **State Management**: React Context API
- **UI Components**: Custom components with Ionicons
- **Styling**: StyleSheet with dynamic theming
- **Theme**: Light/Dark mode support

## Getting Started

```bash
# Install dependencies
npm install

# Start the development server
npx expo start

# Run on iOS
npx expo start --ios

# Run on Android
npx expo start --android
```

## Project Structure

```
app/
├── (tabs)/          # Main tab navigation
│   ├── home.tsx     # Dashboard
│   ├── social.tsx   # Social feed
│   ├── community.tsx # Community projects
│   ├── transactions.tsx # Transaction history
│   └── accounts.tsx # Account management
├── auth/            # Authentication screens
├── payment/         # Payment flows
├── messages/        # Messaging system
├── kyc/            # Verification flows
└── admin/          # Admin features

components/         # Reusable components
contexts/          # React contexts (Theme, Auth)
constants/         # Colors, Images, etc.
```

## Key Features Implementation

### Theme System
The app supports light and dark themes with a toggle in the header. Colors are managed through the ThemeContext.

### Authentication Flow
1. Welcome screen with Login/Signup
2. PIN entry (6 digits)
3. OTP verification
4. KYC verification (4-step process)
5. Main dashboard access

### Payment Flow
1. Select payment type (Send/Receive/QR)
2. Choose linked bank account
3. Select transfer method
4. Confirm and execute

### Benefit Tier System
Users progress through 5 tiers based on contribution:
- Basic
- Skilled
- Advanced
- Expert
- Official

"Level of Benefit = Level of Contribution"

## API Integration Ready

The app is structured to integrate with:
- Brankas
- UnionBank
- ADB
- RippleNet / XRPL
- mBridge (BIS-compatible)
- QRPH
- GCash, GoTyme, PayPal, Payoneer, Alipay, Wise, Stripe, Coins.ph

## Compliance

Built with consideration for:
- Anti-Financial Accounts Scamming Act
- AMLA (Anti-Money Laundering Act)
- Data Privacy Act
- ISO 20022 standards
- BIS mBridge messaging

## Future Enhancements

- Backend API integration
- Real-time blockchain ledger (ISET XRPL)
- Offline-first architecture with sync
- AI-powered accounting and analytics
- 13-Moon Natural Time Calendar integration
- Advanced admin controls
- Push notifications via Firebase

## License

Proprietary - ISET Fiduciary Finance Platform

# TV2NJ TopstepX Trading Bot

## Overview

TV2NJ (TradingView to NinjaTrader) is a sophisticated automated trading bot that bridges TradingView signals with NinjaTrader execution, now enhanced with TopstepX integration. This powerful addon enables traders to execute their TradingView strategies seamlessly on TopstepX funded accounts through NinjaTrader.

## Key Features

### 1. **Multi-Platform Integration**
- **TradingView Signals**: Receives real-time trading signals from TradingView via webhooks
- **NinjaTrader Execution**: Executes trades directly in NinjaTrader 8
- **TopstepX API Integration**: Native support for TopstepX funded trading accounts
- **WebSocket Communication**: Real-time signal relay through secure WebSocket connections

### 2. **Advanced Signal Processing**
- **Smart Signal Routing**: Automatically routes signals to appropriate accounts based on signal parameters
- **Symbol Mapping**: Intelligent conversion between TradingView and TopstepX contract formats
- **Multi-Account Support**: Trade multiple accounts simultaneously with account-specific rules
- **Signal Filtering**: Filter signals by account, symbol, or custom parameters

### 3. **Risk Management**
- **Position Limits**: Set maximum positions per symbol and account
- **Daily P&L Limits**: Automatic trading halt when profit/loss targets are reached
- **OCO Orders**: One-Cancels-Other order support for automatic stop-loss and take-profit
- **Account Protection**: Designated protected accounts with special trading rules
- **Micro Futures Support**: Built-in protection for micro futures contracts

### 4. **Trading Controls**
- **Time-Based Trading**: Configure specific trading hours for automated execution
- **Directional Control**: Enable/disable long and short positions independently
- **Reversal Trading**: Support for position reversal strategies
- **Manual Override**: Pause/resume signal processing at any time
- **Real-Time Monitoring**: Live logs and position tracking

### 5. **TopstepX Specific Features**
- **API Key Authentication**: Secure authentication using TopstepX API credentials
- **Account Filtering**: Display only tradable accounts
- **Contract Search**: Automatic contract resolution for futures symbols
- **Balance Display**: Real-time account balance and position information
- **Multiple Account Management**: Handle multiple TopstepX accounts from one interface

## Technical Advantages

### 1. **Reliability**
- Automatic reconnection on disconnection
- Token validation and refresh
- Error handling with detailed logging
- Persistent settings storage

### 2. **Performance**
- Asynchronous order execution
- Efficient WebSocket message processing
- Minimal latency signal relay
- Optimized API calls

### 3. **Flexibility**
- Configurable for any TradingView strategy
- Support for market, limit, and stop orders
- Custom signal parameters (SL, TP, quantity)
- Per-account trading rules

### 4. **Security**
- Encrypted API communication
- Secure credential storage
- No exposure of sensitive data in logs
- Token-based authentication

## Use Cases

1. **Prop Trading**: Perfect for TopstepX funded traders automating their strategies
2. **Multi-Strategy Trading**: Run multiple TradingView strategies on different accounts
3. **Risk Management**: Implement sophisticated risk rules across all positions
4. **Signal Services**: Follow professional traders' signals automatically
5. **Backtesting to Live**: Seamlessly transition from TradingView backtests to live trading

## Technical Architecture

```
TradingView Alert → Webhook → ExcellGen Relay → WebSocket → TV2NJ → NinjaTrader → TopstepX API
```

### Components:
- **Signal Parser**: Processes JSON signals with custom parameters
- **Order Manager**: Handles order placement and modification
- **Account Manager**: Manages multiple account connections
- **Risk Engine**: Enforces position limits and P&L rules
- **UI System**: Tabbed interface for configuration and monitoring

## Configuration Options

- **Connection Settings**: API URLs, authentication credentials
- **Trading Parameters**: Stop loss, take profit, position sizing
- **Account Selection**: Choose specific accounts for trading
- **Symbol Mapping**: Configure symbol conversions
- **Risk Limits**: Set daily and per-trade limits
- **Time Restrictions**: Define trading hours

## Getting Started

1. Install the TV2NJ addon in NinjaTrader 8
2. Configure TopstepX API credentials
3. Set up TradingView webhooks with ExcellGen relay
4. Configure trading parameters and risk limits
5. Connect and start receiving signals

## System Requirements

- NinjaTrader 8
- TopstepX API access ($29/month with 50% discount code: "topstep")
- TradingView (Pro or higher for webhooks)
- Windows 10/11
- .NET Framework 4.8 or higher
- Stable internet connection

## Support

- Comprehensive logging for troubleshooting
- Real-time connection status monitoring
- Detailed error messages
- Signal replay capabilities for testing

---

*TV2NJ TopstepX Bot - Bridging the gap between strategy and execution*

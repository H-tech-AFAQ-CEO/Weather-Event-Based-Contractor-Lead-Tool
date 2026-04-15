# StormLead — Weather Event-Based Contractor Lead Tool

A real-time weather intelligence platform that automatically converts severe storm events into qualified contractor leads using live NOAA data and AI-powered business discovery.

## 🌟 Features

### Real-Time Storm Tracking
- **NOAA/NWS Integration**: Live weather alerts and storm data
- **Intelligent Parsing**: Extracts wind speed, hail size, and precipitation from weather descriptions
- **Severity Ranking**: Dynamic scoring based on storm intensity and recency
- **Storm Visualization**: Interactive map with impact zones and storm tracks

### Advanced Filtering
- **Geographic Filters**: State, region, and ZIP code proximity search
- **Severity Filters**: Wind speed, hail size, and storm severity levels
- **Time Range**: Filter storms from last 24-72 hours
- **Dynamic Sorting**: Real-time ranking by severity and recency

### Contractor Lead Generation
- **Google Places API**: Real contractor discovery in affected areas
- **Apollo.io Integration**: Lead enrichment with contact details and emails
- **Smart Sorting**: By rating, distance, and review count
- **Multiple Categories**: Roofing, plumbing, electrical, HVAC, general contractors

### Data Management
- **Save/Export**: Persistent lead storage and CSV export
- **Auto-Refresh**: Real-time storm data updates every 5 minutes
- **Multi-Source**: Combines demo data with real API responses
- **Offline Support**: Cached data for continued functionality

## 🚀 Quick Start

1. **Open** `index.html` in your browser
2. **Add API Keys** in Settings (optional for demo):
   - NOAA/NWS API Token (for real weather data)
   - Google Places API Key (for real contractor data)
   - Apollo.io API Key (for lead enrichment)
3. **Monitor Storms** on the interactive map
4. **Generate Leads** by clicking on any storm
5. **Export Data** as CSV for external use

## 📊 API Integration

### NOAA/NWS Weather Service
```javascript
// Fetches active weather alerts
https://api.weather.gov/alerts/active?area=US
```

### Google Places API
```javascript
// Searches for contractors near storm locations
https://maps.googleapis.com/maps/api/place/nearbysearch/json
```

### Apollo.io API
```javascript
// Enriches contractor data with contact details
https://api.apollo.io/v1/mixed_people/search
```

## 🎯 Use Cases

### For Contractors
- **Lead Generation**: Receive instant notifications for jobs in your area
- **Competitive Intelligence**: Monitor storm activity and competitor presence
- **Resource Planning**: Anticipate demand spikes based on weather patterns

### For Insurance Companies
- **Claims Management**: Identify affected areas and potential claim volumes
- **Vendor Coordination**: Connect with local contractors for rapid response
- **Risk Assessment**: Analyze storm patterns and historical data

### For Emergency Services
- **Resource Allocation**: Deploy teams based on storm severity and affected areas
- **Public Safety**: Identify high-risk zones and vulnerable populations
- **Coordination**: Connect with local service providers

## 🛠 Technical Architecture

### Frontend (Current)
- **HTML5/CSS3/JavaScript**: Modern responsive interface
- **Leaflet.js**: Interactive mapping with custom markers
- **Lucide Icons**: Clean, consistent iconography
- **LocalStorage**: Client-side data persistence

### Backend (Planned)
- **Node.js/Express**: RESTful API server
- **PostgreSQL**: Storm and lead data management
- **Redis**: Real-time caching and session management
- **WebSocket**: Live updates and notifications

### Data Sources
- **NOAA/NWS**: Primary weather data source
- **Google Places**: Contractor business information
- **Apollo.io**: Contact and company enrichment
- **OpenStreetMap**: Geographic and mapping data

## 📈 Performance Features

### Caching Strategy
- **5-minute cache** for weather data
- **Session storage** for user preferences
- **LocalStorage** for saved leads
- **Smart refresh** based on visibility state

### Optimization
- **Lazy loading** for map tiles
- **Debounced searches** for better UX
- **Efficient filtering** with indexed data
- **Progressive enhancement** with fallbacks

## 🔧 Configuration

### Environment Variables
```bash
# API Keys (add in Settings UI)
NOAA_API_KEY=your_noaa_api_key
GOOGLE_PLACES_API_KEY=your_google_api_key
APOLLO_API_KEY=your_apollo_api_key
```

### Default Settings
- **Search Radius**: 25 miles (configurable)
- **Auto-refresh**: 5 minutes (configurable)
- **Cache Duration**: 5 minutes for weather data
- **Max Results**: 50 contractors per storm

## 🎨 UI Components

### Map Features
- **Storm Markers**: Color-coded by severity
- **Impact Zones**: Radius-based visualization
- **Storm Tracks**: Predicted movement patterns
- **Fullscreen Mode**: Immersive monitoring experience

### Data Tables
- **Sortable Columns**: Click headers to sort
- **Rich Data**: Contact info, ratings, distance
- **Bulk Actions**: Save or export multiple leads
- **Status Indicators**: Visual feedback for actions

## 📱 Responsive Design

- **Desktop**: Full-featured interface with sidebar
- **Tablet**: Optimized layout with touch controls
- **Mobile**: Simplified interface with swipe gestures
- **Progressive**: Works on all modern browsers

## 🔒 Security & Privacy

- **Client-side Only**: No server data transmission
- **API Key Storage**: Encrypted localStorage
- **CORS Handling**: Secure API communication
- **Data Sanitization**: XSS prevention

## 🚧 Development Roadmap

### Phase 1: Backend Implementation
- [ ] Node.js/Express server setup
- [ ] PostgreSQL database schema
- [ ] API endpoint development
- [ ] WebSocket real-time updates

### Phase 2: Advanced Features
- [ ] Machine learning storm prediction
- [ ] Automated lead scoring
- [ ] Email/SMS notifications
- [ ] Mobile app development

### Phase 3: Enterprise Features
- [ ] Multi-user accounts
- [ ] Role-based permissions
- [ ] Analytics dashboard
- [ ] White-label solutions

## 📄 License

MIT License - Feel free to use, modify, and distribute for commercial purposes.

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Add tests if applicable
5. Submit a pull request

## 📞 Support

For questions, support, or custom development:
- **Documentation**: Check this README file
- **Demo**: Open `index.html` in browser
- **Issues**: Report bugs via GitHub issues

---

**Transform weather events into business opportunities with StormLead** 🌪️💼

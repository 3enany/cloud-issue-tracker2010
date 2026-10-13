# Request Flow

## Create Issue
User → Frontend form → POST /api/issues → API validation → Data layer
 ← Render created issue ← 201 + JSON ←───────────────┘

## View Issues

Page load → GET /api/issues → API → Data layer
 ← Render list ← 200 + JSON array ←───┘

## Update Issues

 ton → PATCH /api/issues/{id}/status → API validation → Data layer
 ← Re-render issue ← 200 + updated JSON ←──────────┘ 


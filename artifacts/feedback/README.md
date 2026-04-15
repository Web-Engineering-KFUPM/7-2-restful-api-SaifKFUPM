# Lab | songs-api-mongoose-crud | Autograding Summary

- Student: `student`
- ✅ Found `7-2-restful-api/server/index.js`.
- ✅ Model file found: `server/models/song.model.js`
- Late submission (latest repo commit is after due): 10/20. (HEAD: unknown @ unknown)
- Due (Riyadh): `2025-11-19T23:59:00+03:00`

- Repo HEAD commit:
  - SHA: `unknown`
  - Author: `unknown` <unknown>
  - Time (UTC ISO): `unknown`

- Status: **1** (0=on time, 1=late, 2=no submission/empty)
- Run: `2026-04-15T06:40:48.955Z`

## Marks Breakdown

| Item | Marks |
|------|------:|
| TODO 2: Schema & Model (Song) | 15/15 |
| TODO 3: POST /api/songs | 15/15 |
| TODO 4: GET /api/songs | 15/15 |
| TODO 5: PUT /api/songs/:id | 15/15 |
| TODO 6: DELETE /api/songs/:id | 20/20 |
| Submission | 10/20 |

## Total Marks

**90 / 100**

## Detailed Feedback

### TODO 2: Schema & Model (Song)
- ✅ Imports mongoose
- ✅ Defines a mongoose.Schema
- ✅ Schema includes title field
- ✅ title is required
- ✅ Schema includes artist field
- ✅ artist is required
- ✅ Schema includes year (Number)
- ✅ Creates & exports model named "Song"

### TODO 3: POST /api/songs
- ✅ Defines POST "/api/songs"
- ✅ Uses async handler
- ✅ Reads JSON body (title, artist, year)
- ✅ Inserts song into DB (Song.create/save)
- ✅ Responds with 201 + created song JSON
- ✅ On error responds 400 + {message}

### TODO 4: GET /api/songs
- ✅ Defines GET "/api/songs"
- ✅ Uses Song.find()
- ✅ Sorts newest first (createdAt desc)
- ✅ Returns JSON list
- ✅ (Optional) Defines GET "/api/songs/:id"
- ✅ (Optional) Uses Song.findById()
- ✅ (Optional) 404 {message:"Song not found"} when missing

### TODO 5: PUT /api/songs/:id
- ✅ Defines PUT "/api/songs/:id"
- ✅ Uses Song.findByIdAndUpdate()
- ✅ Passes { new: true }
- ✅ Passes { runValidators: true }
- ✅ If not found -> 404 {message:"Song not found"}
- ✅ On validation error -> 400 {message}

### TODO 6: DELETE /api/songs/:id
- ✅ Defines DELETE "/api/songs/:id"
- ✅ Uses Song.findByIdAndDelete()
- ✅ If not found -> 404 {message:"Song not found"}
- ✅ On success -> 204 No Content

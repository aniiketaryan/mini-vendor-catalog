# mini-vendor-catalog
# Mini Vendor Catalog Manager

A full-stack vendor catalog app: vendors can add, view, and delete products in a Swiggy Instamart-style web interface. Built with React (Vite + Tailwind CSS), Express.js, MongoDB Atlas. Features live updating, product grid, swift backend, and automatic UI refresh.

**Demo:** [Add your Vercel app link]
**API:** [Add your Render app link]

### Features
- Product grid (Swiggy-style)
- Add, view, and delete instantly
- Clean modern UI with Tailwind
- All data stored in MongoDB Cloud

### Tech
- Frontend: React (Vite), Tailwind CSS, Axios
- Backend: Express.js, Mongoose
- Database: MongoDB Atlas
- Deployment: Vercel (frontend), Render (backend)

### Local Development
1. Clone repo: `git clone ...`
2. Backend:
   - `cd backend`
   - `cp .env.example .env` (fill in your MongoDB connection string)
   - `npm install`
   - `npm run dev`
3. Frontend:
   - `cd ../frontend`
   - Add `.env` with `VITE_API_BASE_URL=http://localhost:5000`
   - `npm install`
   - `npm run dev`

### API Endpoints
- `GET /api/products`: list all products
- `POST /api/products`: add a product `{ name, description, price }`
- `DELETE /api/products/:id`: delete product by ID

---

**Repo Description:**
> Mini Vendor Catalog Manager — Swiggy Instamart-style web app. React frontend, Express/MongoDB backend. Add/view/delete products. Clean, modern, and easy to deploy.

---

## Common Errors and Fixes
- **repo not found**: Make sure you created the repo, and remote URL matches your GitHub.
- **src refspec main does not match any**: Make your first commit before pushing (`git add .; git commit -m "init"`).
- **Command not found (npm, npx, git)**: Install Node.js + git from official sites.
- **Database errors**: Check MongoDB Atlas connection string, user rights, and IP whitelist.
- **CORS errors**: Ensure `app.use(cors())` is in the backend server.js.
- **Frontend can't reach backend**: Make sure both are running locally, and `.env` points to correct port.

---

You're all set! If you hit a specific error, paste it here and I'll walk you through the exact solution. If you want more Swiggy-style features (like images, search, login), let me know and we can build out detailed components together.

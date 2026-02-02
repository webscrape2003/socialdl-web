<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>CapCut Template Downloader</title>
    <link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;600;800&display=swap" rel="stylesheet">
    <style>
        :root { --primary: #00f2ea; --secondary: #ff0050; --bg: #0a0a0a; --card: #121212; --text: #ffffff; }
        body { background-color: var(--bg); color: var(--text); font-family: 'Plus Jakarta Sans', sans-serif; margin: 0; }
        .header { padding: 20px; background: #000; border-bottom: 1px solid #222; position: sticky; top: 0; z-index: 1000; }
        .search-box { max-width: 600px; margin: 0 auto; display: flex; gap: 10px; background: #1a1a1a; padding: 5px; border-radius: 12px; border: 1px solid #333; }
        input { flex: 1; background: transparent; border: none; color: white; padding: 12px; outline: none; font-size: 1rem; }
        button { background: var(--primary); color: #000; border: none; padding: 0 20px; border-radius: 8px; font-weight: 700; cursor: pointer; transition: 0.2s; }
        button:hover { opacity: 0.8; }
        .container { max-width: 1200px; margin: 30px auto; padding: 0 15px; }
        .section-title { font-size: 1.4rem; font-weight: 800; margin-bottom: 25px; color: #fff; border-left: 5px solid var(--secondary); padding-left: 15px; }
        .movie-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(280px, 1fr)); gap: 20px; }
        .movie-card { background: var(--card); border-radius: 12px; overflow: hidden; transition: 0.3s; border: 1px solid #222; position: relative; }
        .movie-card:hover { transform: translateY(-8px); border-color: var(--primary); }
        .badge-container { position: absolute; top: 10px; left: 10px; display: flex; flex-wrap: wrap; gap: 5px; z-index: 10; }
        .badge { font-size: 0.65rem; font-weight: 800; padding: 4px 8px; border-radius: 4px; text-transform: uppercase; color: white; }
        .badge.quality { background: var(--secondary); }
        .image-container { position: relative; width: 100%; padding-top: 56.25%; background: #1a1a1a; }
        .movie-card img { position: absolute; top: 0; left: 0; width: 100%; height: 100%; object-fit: cover; }
        .card-info { padding: 15px; }
        .card-title { font-size: 0.95rem; font-weight: 600; color: #fff; margin-bottom: 10px; display: -webkit-box; -webkit-line-clamp: 2; -webkit-box-orient: vertical; overflow: hidden; }
        .download-btn { display: block; width: 100%; padding: 10px; background: #333; color: white; text-align: center; text-decoration: none; border-radius: 6px; font-size: 0.8rem; font-weight: 600; margin-top: 8px; transition: 0.3s; }
        .download-btn:hover { background: var(--primary); color: #000; }
        #loader { display: none; text-align: center; padding: 40px; color: var(--primary); font-weight: 800; }
    </style>
</head>
<body>

<div class="header">
    <div class="search-box">
        <input type="text" id="searchInput" placeholder="Paste CapCut URL here...">
        <button id="searchBtn" onclick="fetchCapcut()">FETCH</button>
    </div>
</div>

<div class="container">
    <div class="section-title" id="statusText">Template Results</div>
    <div id="loader">EXTRACTING MEDIA...</div>
    <div class="movie-grid" id="movieGrid"></div>
</div>

<script>
    const API_KEY = "vajira-1qg3lqmr60-1768268975394";

    async function fetchCapcut() {
        const urlInput = document.getElementById('searchInput').value.trim();
        const grid = document.getElementById('movieGrid');
        const loader = document.getElementById('loader');
        const status = document.getElementById('statusText');

        if (!urlInput) return;

        grid.innerHTML = '';
        loader.style.display = 'block';
        status.innerText = `Processing CapCut Link...`;

        try {
            const apiUrl = `https://vajira-official-apis.vercel.app/api/capcut?apikey=${API_KEY}&url=${encodeURIComponent(urlInput)}`;
            const response = await fetch(apiUrl);
            const res = await response.json();

            loader.style.display = 'none';

            if (res.status && res.data) {
                const item = res.data;
                const author = item.author || "Unknown Creator";
                const title = item.title || "CapCut Template";
                const thumb = item.thumbnail;
                
                let html = '';
                
                // We map through the 'medias' array to show different quality versions
                item.medias.forEach(media => {
                    html += `
                        <div class="movie-card">
                            <div class="badge-container">
                                <span class="badge quality">${media.quality}</span>
                            </div>
                            <div class="image-container">
                                <img src="${thumb}" alt="thumbnail">
                            </div>
                            <div class="card-info">
                                <div class="card-title">${title}</div>
                                <div style="color: #888; font-size: 0.75rem; margin-bottom: 10px;">By ${author}</div>
                                <a href="${media.url}" class="download-btn" target="_blank">DOWNLOAD ${media.extension.toUpperCase()}</a>
                            </div>
                        </div>`;
                });
                
                grid.innerHTML = html;
                status.innerText = `Result for: ${title}`;
            } else {
                status.innerText = "Failed to fetch template. Check URL.";
            }
        } catch (err) {
            loader.style.display = 'none';
            status.innerText = "API Connection Error";
            console.error(err);
        }
    }

    document.getElementById('searchInput').addEventListener('keypress', e => { if(e.key === 'Enter') fetchCapcut(); });
</script>
</body>
</html>

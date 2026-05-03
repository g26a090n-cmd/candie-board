<!DOCTYPE html>
<html lang="ja">
<head>
<meta charset="UTF-8">
<title>掲示板</title>

<link href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap" rel="stylesheet">

<style>
body {
    font-family: sans-serif;
    background: #fff7f0;
    margin: 0;
    padding: 20px;
}

.logo {
    font-family: 'Pacifico', cursive;
    color: #ff7a00;
    font-size: 2em;
}

.container {
    max-width: 700px;
    margin: auto;
}

.post {
    background: white;
    padding: 15px;
    margin: 10px 0;
    border-left: 5px solid #ff7a00;
    cursor: pointer;
}

input, textarea, select {
    width: 100%;
    margin: 5px 0;
    padding: 8px;
}

button {
    background: #ff7a00;
    color: white;
    border: none;
    padding: 10px;
    margin-top: 5px;
    cursor: pointer;
}

.section-title {
    color: #ff7a00;
    border-bottom: 2px solid #ff7a00;
    margin-top: 30px;
}
</style>
</head>

<body>

<div class="container">
<div class="logo">candle</div>

<h2>投稿する</h2>

<select id="type">
    <option value="news">お知らせ</option>
    <option value="event">イベント</option>
    <option value="minutes">議事録</option>
</select>

<input id="title" placeholder="タイトル">
<textarea id="content" placeholder="内容"></textarea>

<button onclick="addPost()">投稿</button>

<hr>

<div id="app"></div>

</div>

<script>
let posts = JSON.parse(localStorage.getItem("posts") || "[]");

function save() {
    localStorage.setItem("posts", JSON.stringify(posts));
}

function addPost() {
    const post = {
        id: Date.now(),
        type: document.getElementById("type").value,
        title: document.getElementById("title").value,
        content: document.getElementById("content").value,
        date: new Date().toISOString().slice(0,10)
    };

    posts.push(post);
    save();
    location.reload();
}

function deletePost(id) {
    posts = posts.filter(p => p.id !== id);
    save();
    location.reload();
}

function render() {
    const app = document.getElementById("app");

    const types = {
        news: "お知らせ",
        event: "イベント情報",
        minutes: "議事録"
    };

    let html = "";

    Object.keys(types).forEach(type => {
        html += `<h3 class="section-title">${types[type]}</h3>`;

        posts
        .filter(p => p.type === type)
        .sort((a,b)=> new Date(b.date) - new Date(a.date))
        .forEach(p => {
            html += `
                <div class="post">
                    <b>${p.title}</b><br>
                    <small>${p.date}</small>
                    <button onclick="deletePost(${p.id})">削除</button>
                </div>
            `;
        });
    });

    app.innerHTML = html;
}

render();
</script>

</body>
</html>

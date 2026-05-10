// api/gemini.js
export default async function handler(req, res) {
    // 设置跨域头，允许其他网站调用你的 API
    res.setHeader('Access-Control-Allow-Origin', '*');
    
    // 只处理 POST 请求
    if (req.method !== 'POST') {
        return res.status(200).end();
    }

    const { message } = req.body;
    const apiKey = process.env.GEMINI_API_KEY; // 密钥从环境变量读取

    const url = `https://generativelanguage.googleapis.com/v1beta/models/gemini-2.5-flash:generateContent?key=${apiKey}`;

    try {
        const response = await fetch(url, {
            method: 'POST',
            headers: { 'Content-Type': 'application/json' },
            body: JSON.stringify({
                contents: [{ parts: [{ text: message }] }],
            }),
        });
        const data = await response.json();
        const reply = data.candidates[0].content.parts[0].text;
        
        res.status(200).json({ reply });
    } catch (error) {
        res.status(500).json({ error: '请求失败' });
    }
}
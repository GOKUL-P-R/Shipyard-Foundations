<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>CI/CD Assignment</title>

<style>
    body {
        margin: 0;
        font-family: Arial, sans-serif;
        background: linear-gradient(270deg, #0f172a, #1e3a8a, #0f172a);
        background-size: 600% 600%;
        animation: gradientBG 10s ease infinite;
        color: white;
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;                                                            
    }

    @keyframes gradientBG {
        0% { background-position: 0% 50%; }
        50% { background-position: 100% 50%; }
        100% { background-position: 0% 50%; }
    }
    
                                                                                                                        
    .card {
        background: rgba(255, 255, 255, 0.1);
        padding: 30px;
        border-radius: 15px;
        text-align: center;
        box-shadow: 0 10px 25px rgba(0,0,0,0.4);
        backdrop-filter: blur(10px);
        animation: fadeIn 2s ease;
    }
                                                                                                                                                                                        
    @keyframes fadeIn {
        from {
            opacity: 0;
            transform: translateY(30px);
        }
        to {
            opacity: 1;                                                                                                                                         
            transform: translateY(0)                             
        }
    }
    
    h1 {
        margin-bottom: 10px;
        animation: slideIn 1.5s ease;
    }
                                                                                                                                                                                                                                                                                                        
    @keyframes slideIn {
        from {
            transform: translateX(-50px);
            opacity: 0;
        }
        to {
            transform: translateX(0);
            opacity: 1;
        }
    }
                                                                                                                                                                                                                                                                                                                                                                                                
    .btn {
        margin-top: 15px;
        padding: 10px 20px;
        background: #22c55e;
        color: white;
        border: none;
        border-radius: 20px;
        cursor: pointer;
        transition: transform 0.3s, box-shadow 0.3s;
    }
                                                                                                                                                                                                                                                                                                                                                                                                                                                                        
    .btn:hover {
        transform: scale(1.1);
        box-shadow: 0 0 15px #22c55e;
    }
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                
</style>
</head>
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                
<body>
    <div class="card">
        <h1>🚀 CI/CD Pipeline Basics</h1>
        <p>Website deployed using GitHub Actions + GitHub Pages</p>
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    
        <p><strong>Name:</strong> GOKUL P R</p>
        <p><strong>MUID:</strong> gokulpr-1@mulearn</p>
                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    
        <button class="btn">Deployment Successful ✅</button>
    </div>
</body>
</html>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               </html>

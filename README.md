# Zac-sales-page
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Stop Training Around Pain - Move Like You Were Born To</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        
        html, body {
            overflow-x: hidden;
        }
        
        body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif;
            line-height: 1.6;
            color: #2c3e50;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
        }
        
        .container {
            width: 100%;
            max-width: 800px;
            margin: 0 auto;
            padding: 0 20px;
        }
        
        .hero-section {
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            color: white;
            padding: 60px 0;
            text-align: center;
        }
        
        .preheader {
            font-size: 1.1em;
            margin-bottom: 20px;
            opacity: 0.9;
            text-transform: uppercase;
            letter-spacing: 2px;
            font-weight: 600;
        }
        
        .main-header {
            font-size: 3.5em;
            font-weight: 900;
            margin-bottom: 20px;
            line-height: 1.1;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.3);
        }
        
        .subheader {
            font-size: 1.4em;
            margin-bottom: 40px;
            opacity: 0.95;
            font-weight: 400;
        }
        
        .vsl-container {
            margin: 40px 0;
            position: relative;
            display: inline-block;
            max-width: 500px;
            width: 100%;
        }
        
        .vsl-thumbnail {
            width: 100%;
            height: 280px;
            background: linear-gradient(rgba(0,0,0,0.3), rgba(0,0,0,0.3)), url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 500 280"><rect fill="%23667eea" width="500" height="280"/><text x="250" y="120" text-anchor="middle" fill="white" font-size="16" font-family="Arial">Watch: The 3-Minute Movement</text><text x="250" y="140" text-anchor="middle" fill="white" font-size="16" font-family="Arial">Assessment That Reveals</text><text x="250" y="160" text-anchor="middle" fill="white" font-size="16" font-family="Arial">Your Hidden Pain Triggers</text></svg>');
            background-size: cover;
            background-position: center;
            border-radius: 15px;
            position: relative;
            cursor: pointer;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            box-shadow: 0 15px 40px rgba(0,0,0,0.3);
            border: 3px solid rgba(255,255,255,0.2);
        }
        
        .vsl-thumbnail:hover {
            transform: translateY(-5px);
            box-shadow: 0 20px 50px rgba(0,0,0,0.4);
        }
        
        .play-button-overlay {
            position: absolute;
            top: 50%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 80px;
            height: 80px;
            background: rgba(255,107,107,0.9);
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: all 0.3s ease;
        }
        
        .vsl-thumbnail:hover .play-button-overlay {
            background: rgba(255,107,107,1);
            transform: translate(-50%, -50%) scale(1.1);
        }
        
        .play-button {
            width: 0;
            height: 0;
            border-left: 25px solid white;
            border-top: 15px solid transparent;
            border-bottom: 15px solid transparent;
            margin-left: 5px;
        }
        
        .vsl-duration {
            position: absolute;
            bottom: 15px;
            right: 15px;
            background: rgba(0,0,0,0.8);
            color: white;
            padding: 5px 10px;
            border-radius: 5px;
            font-size: 0.9em;
            font-weight: 600;
        }
        
        .primary-cta {
            background: linear-gradient(135deg, #ff6b6b, #ee5a24);
            color: white;
            padding: 20px 40px;
            font-size: 1.3em;
            font-weight: 700;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            transition: all 0.3s ease;
            text-transform: uppercase;
            letter-spacing: 1px;
            box-shadow: 0 8px 25px rgba(0,0,0,0.2);
            margin-top: 30px;
        }
        
        .primary-cta:hover {
            transform: translateY(-3px);
            box-shadow: 0 12px 35px rgba(0,0,0,0.3);
        }
        
        .content-section {
            background: white;
            padding: 80px 0;
        }
        
        .section-header {
            font-size: 2.5em;
            font-weight: 800;
            margin-bottom: 30px;
            text-align: center;
            color: #2c3e50;
        }
        
        .content-text {
            font-size: 1.2em;
            margin-bottom: 25px;
            line-height: 1.7;
        }
        
        .content-text strong {
            font-weight: 700;
            color: #e74c3c;
        }
        
        .content-text em {
            font-style: italic;
            color: #3498db;
        }
        
        .bullet-list {
            margin: 30px 0;
        }
        
        .bullet-item {
            background: #f8f9fa;
            padding: 20px;
            margin-bottom: 15px;
            border-radius: 10px;
            border-left: 4px solid #667eea;
        }
        
        .bullet-item strong {
            color: #2c3e50;
            font-weight: 700;
        }
        
        .testimonial {
            background: linear-gradient(135deg, #74b9ff, #0984e3);
            color: white;
            padding: 30px;
            border-radius: 15px;
            margin: 30px 0;
            font-style: italic;
            font-size: 1.1em;
        }
        
        .testimonial-author {
            text-align: right;
            margin-top: 15px;
            font-weight: 600;
            opacity: 0.9;
        }
        
        .offer-section {
            background: linear-gradient(135deg, #2d3436, #636e72);
            color: white;
            padding: 80px 0;
        }
        
        .offer-section .section-header {
            color: white;
        }
        
        .pricing-card {
            background: white;
            color: #2c3e50;
            padding: 40px;
            border-radius: 15px;
            margin: 30px 0;
            box-shadow: 0 15px 50px rgba(0,0,0,0.1);
        }
        
        .price {
            font-size: 2.5em;
            font-weight: 900;
            color: #e74c3c;
            text-align: center;
            margin-bottom: 20px;
        }
        
        .guarantee {
            background: #00b894;
            color: white;
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            font-weight: 600;
            margin: 30px 0;
        }
        
        .faq-section {
            background: #f8f9fa;
            padding: 80px 0;
        }
        
        .faq-item {
            background: white;
            padding: 30px;
            margin-bottom: 20px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.08);
        }
        
        .faq-question {
            font-weight: 700;
            font-size: 1.2em;
            margin-bottom: 15px;
            color: #2c3e50;
        }
        
        .urgency-box {
            background: linear-gradient(135deg, #ff7675, #d63031);
            color: white;
            padding: 30px;
            border-radius: 15px;
            text-align: center;
            margin: 40px 0;
            font-size: 1.1em;
            font-weight: 600;
        }
        
        @media (max-width: 1024px) {
            .main-header {
                font-size: 3em;
            }
            
            .container {
                padding: 0 15px;
            }
        }
        
        @media (max-width: 768px) {
            .main-header {
                font-size: 2.2em;
            }
            
            .subheader {
                font-size: 1.2em;
            }
            
            .content-section, .offer-section, .faq-section {
                padding: 50px 0;
            }
            
            .section-header {
                font-size: 2em;
            }
            
            .primary-cta {
                padding: 15px 30px;
                font-size: 1.1em;
            }
            
            .vsl-thumbnail {
                height: 200px;
            }
            
            .play-button-overlay {
                width: 60px;
                height: 60px;
            }
            
            .play-button {
                border-left: 20px solid white;
                border-top: 12px solid transparent;
                border-bottom: 12px solid transparent;
            }
        }
    </style>
</head>
<body>

<!-- HERO SECTION -->
<div class="hero-section">
    <div class="container">
        <div class="preheader">For Athletes, Desk Warriors & Anyone Tired of Training Around Pain</div>
        
        <h1 class="main-header">Move Pain-Free in 6 Weeks Without Endless Mobility Drills</h1>
        
        <p class="subheader">Finally... a proven system that fixes your movement restrictions so you can train hard again <strong>without</strong> spending hours on random stretches that don't stick</p>
        
        <div class="vsl-container">
            <div class="vsl-thumbnail">
                <div class="play-button-overlay">
                    <div class="play-button"></div>
                </div>
                <div class="vsl-duration">3:47</div>
            </div>
        </div>
        
        <button class="primary-cta">Apply For Your Assessment Call</button>
    </div>
</div>

<!-- PROBLEM IDENTIFICATION -->
<div class="content-section">
    <div class="container">
        <h2 class="section-header">You're One Squat Away From Wincing Again...</h2>
        
        <p class="content-text">That sharp twinge in your hip. The shoulder that screams when you reach overhead. The knee that makes you think twice about every lunge.</p>
        
        <p class="content-text">You've tried everything...</p>
        
        <p class="content-text">Scrolled through <strong>hundreds</strong> of mobility videos on Instagram. Spent 45 minutes doing foam rolling routines that made you feel good for... what... 20 minutes?</p>
        
        <p class="content-text">You've worked with trainers who gave you the <em>same cookie-cutter program</em> they give everyone else.</p>
        
        <p class="content-text">And here you are... <strong>still in pain.</strong></p>
        
        <p class="content-text">Still avoiding certain movements. Still wondering if this is just "getting older" or if there's something actually wrong with you.</p>
        
        <p class="content-text">Meanwhile, that voice in your head keeps getting louder: <em>"What if this never gets better? What if I have to give up the activities I love?"</em></p>
        
        <div class="testimonial">
            "I couldn't lift my arm above my head without pain for months. Three sessions with Zac and I was back to full range of motion. The difference was night and day."
            <div class="testimonial-author">- Blake R.</div>
        </div>
        
        <p class="content-text">But here's what nobody tells you about why you're still stuck...</p>
    </div>
</div>

<!-- ORIGIN STORY -->
<div class="content-section" style="background: #f8f9fa;">
    <div class="container">
        <h2 class="section-header">The NBA Discovery That Changes Everything</h2>
        
        <p class="content-text">Three years ago, I was working with a professional basketball player who couldn't figure out why his jump shot felt "off."</p>
        
        <p class="content-text">No pain. No obvious injury. But something was wrong.</p>
        
        <p class="content-text">Every physical therapist he'd seen focused on the shoulder. Every trainer worked on his shooting form.</p>
        
        <p class="content-text">But when I assessed his movement, I found something they all missed...</p>
        
        <p class="content-text"><strong>His thoracic spine was locked up.</strong> Not painful. Not obviously restricted. But it was stealing power from every movement he made.</p>
        
        <p class="content-text">Six weeks later, he was shooting better than he had in two years.</p>
        
        <p class="content-text">That's when it hit me: <em>Most movement problems aren't where you feel them.</em></p>
        
        <p class="content-text">Your shoulder pain might be coming from your ribs. Your hip pain could be your ankle's fault. Your knee issues? Probably your hip flexors.</p>
        
        <p class="content-text">But here's why every other approach fails...</p>
        
        <p class="content-text">They treat symptoms. Not systems.</p>
        
        <p class="content-text">They give you exercises for where it hurts. Not where the problem actually lives.</p>
        
        <p class="content-text">And that's exactly why you're still dealing with this months (or years) later.</p>
    </div>
</div>

<!-- SOLUTION REVELATION -->
<div class="content-section">
    <div class="container">
        <h2 class="section-header">The Movement Chain Assessment That Actually Works</h2>
        
        <p class="content-text">Here's what we do differently...</p>
        
        <p class="content-text">Instead of guessing or giving you generic exercises, we map your entire movement chain to find the <strong>real source</strong> of your restrictions.</p>
        
        <p class="content-text">Think of your body like a bike chain. When one link gets sticky, the whole thing stops working smoothly.</p>
        
        <p class="content-text">Most people (and most trainers) just oil the squeaky link. We find the actual stuck one and fix that instead.</p>
        
        <p class="content-text">The result? Keith hit a jumping PR just 6 months after ACL surgery. Keri went from avoiding squats to hitting depth without pain. Shuai can finally squat without that grinding sensation in his hip.</p>
        
        <div class="bullet-list">
            <div class="bullet-item">
                <strong>Precision Assessment:</strong> We pinpoint exactly which restrictions are causing your pain so you stop wasting time on movements that don't matter
            </div>
            
            <div class="bullet-item">
                <strong>Targeted Protocols:</strong> Custom 6-week programs that address YOUR specific limitations, not some random collection of stretches from social media
            </div>
            
            <div class="bullet-item">
                <strong>Real-Time Feedback:</strong> Video analysis twice per week so you know you're doing it right and actually making progress
            </div>
        </div>
        
        <div class="testimonial">
            "After my ACL surgery, I thought my jumping days were over. Zac's program not only got me back to where I was - I actually hit a PR six months post-surgery."
            <div class="testimonial-author">- Keith M.</div>
        </div>
    </div>
</div>

<!-- PRODUCT INTRODUCTION -->
<div class="content-section" style="background: #f8f9fa;">
    <div class="container">
        <h2 class="section-header">Introducing: The Movement Freedom System</h2>
        
        <p class="content-text">This isn't another collection of mobility drills you'll forget about in two weeks.</p>
        
        <p class="content-text">This is a complete assessment and coaching system designed to identify your specific movement restrictions and eliminate them systematically.</p>
        
        <p class="content-text">Every exercise in your program exists for one reason: to solve a specific limitation that's keeping you from moving the way you want to move.</p>
        
        <p class="content-text">No fluff. No "funky" exercises just because they look cool on Instagram. Just targeted, effective protocols that actually work.</p>
        
        <p class="content-text">Compare that to what you've been doing...</p>
        
        <p class="content-text">Spending 20 minutes foam rolling your IT band (which doesn't even loosen, by the way). Doing pigeon pose for the 47th time this month. Following along with some influencer's "morning mobility routine" that has nothing to do with your actual problems.</p>
        
        <p class="content-text">This is the exact opposite of all that.</p>
        
        <p class="content-text">When you get $500 worth of assessments and programming for the cost of a few personal training sessions, and it actually works...</p>
        
        <p class="content-text">That's what we call a no-brainer.</p>
    </div>
</div>

<!-- OFFER STRUCTURE -->
<div class="offer-section">
    <div class="container">
        <h2 class="section-header">Here's How We Fix Your Movement (And Your Life)</h2>
        
        <div class="pricing-card">
            <h3 style="text-align: center; margin-bottom: 20px; font-size: 1.8em;">PLATINUM PROGRAM</h3>
            <div class="price">$600-750/month</div>
            
            <div class="bullet-list">
                <div class="bullet-item">
                    <strong>Complete Movement Assessment:</strong> 60-minute deep-dive call to map your restrictions and identify the root cause of your pain
                </div>
                
                <div class="bullet-item">
                    <strong>Custom 6-Week Program:</strong> Tailored specifically to YOUR limitations with detailed video demonstrations for every exercise
                </div>
                
                <div class="bullet-item">
                    <strong>Twice-Weekly Video Reviews:</strong> Submit your technique videos and get personalized feedback within 24 hours
                </div>
                
                <div class="bullet-item">
                    <strong>Quarterly Strategy Calls:</strong> 60-minute sessions with Zac himself to troubleshoot, refine, and level up your program
                </div>
                
                <div class="bullet-item">
                    <strong>Exercise Library Access:</strong> Complete video database of movements, progressions, and modifications
                </div>
            </div>
            
            <div class="guarantee">
                <strong>ZERO-RISK GUARANTEE:</strong> If you don't see measurable improvement in your movement and pain levels within 14 days, get every penny back. No questions asked.
            </div>
        </div>
        
        <div class="urgency-box">
            <strong>IMPORTANT:</strong> We only accept 8 new Platinum clients per month to ensure everyone gets the attention they deserve. Current availability: 3 spots remaining for this month.
        </div>
        
        <div style="text-align: center;">
            <button class="primary-cta">Claim Your Assessment Spot Now</button>
        </div>
    </div>
</div>

<!-- FAQ SECTION -->
<div class="faq-section">
    <div class="container">
        <h2 class="section-header">The Questions Everyone Asks (And The Real Answers)</h2>
        
        <div class="faq-item">
            <div class="faq-question">Q: "I've tried everything. How is this different?"</div>
            <p>Because "everything" you've tried was guessing. We don't guess. We assess your specific movement patterns, identify the exact restrictions causing your problems, and build a program around fixing those. It's the difference between throwing spaghetti at the wall and using a GPS.</p>
        </div>
        
        <div class="faq-item">
            <div class="faq-question">Q: "Can this really work if I'm not there in person?"</div>
            <p>Our online clients often get better results than in-person because you're practicing the movements in your actual training environment. Plus, with video analysis twice per week, you get more coaching than most people get in months of in-person sessions.</p>
        </div>
        
        <div class="faq-item">
            <div class="faq-question">Q: "I don't have time for long workouts. Will this work?"</div>
            <p>Perfect. Our programs are designed for busy people. Most sessions take 15-20 minutes. No hour-long mobility routines. No complex setups. Just targeted work that fits your schedule and actually moves the needle.</p>
        </div>
        
        <div class="faq-item">
            <div class="faq-question">Q: "What if I'm too broken/old/out of shape?"</div>
            <p>We've worked with 70-year-olds getting back to hiking and 20-year-olds recovering from surgery. Age doesn't matter. Fitness level doesn't matter. What matters is following a system that's designed for where you are right now, not where you think you should be.</p>
        </div>
        
        <div style="text-align: center; margin-top: 50px;">
            <button class="primary-cta">Stop Training Around Pain - Start Your Assessment</button>
        </div>
    </div>
</div>

<script>
    // Simple click tracking for CTAs
    document.querySelectorAll('.primary-cta').forEach(button => {
        button.addEventListener('click', function() {
            // In a real implementation, this would redirect to your application form
            alert('Redirecting to application form...');
        });
    });
    
    // VSL thumbnail click
    document.querySelector('.vsl-thumbnail').addEventListener('click', function() {
        // In a real implementation, this would open your video
        alert('Video would play here...');
    });
</script>

</body>
</html>

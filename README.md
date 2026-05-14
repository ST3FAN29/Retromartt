<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8"/>
<meta name="viewport" content="width=device-width,initial-scale=1.0"/>
<title>Retro Hub — Premium Digital Services</title>
<meta name="description" content="Buy Discord Nitro, Netflix, Robux, Crunchyroll, Spotify and more at unbeatable prices. Trusted Discord shop. Fast delivery."/>
<meta property="og:title" content="Retro Hub — Premium Digital Services"/>
<meta name="theme-color" content="#c8001a"/>
<link rel="preconnect" href="https://fonts.googleapis.com"/>
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin/>
<link href="https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Syne:wght@400;500;600;700&family=JetBrains+Mono:wght@400;500&display=swap" rel="stylesheet"/>
<style>
/* ── TOKENS ─────────────────────────────────── */
:root{
  --r:#c8001a; --rb:#ff1f35; --rd:#7a000f;
  --rg:rgba(200,0,26,.4); --rgs:rgba(200,0,26,.12);
  --bg:#060606; --bg2:#0c0c0c; --bg3:#111;
  --b:rgba(255,255,255,.07); --br:rgba(200,0,26,.35);
  --t:#ededed; --t2:#888; --t3:#444;
  --fd:'Bebas Neue',sans-serif;
  --fb:'Syne',sans-serif;
  --fm:'JetBrains Mono',monospace;
  --rad:10px; --rad2:16px;
  --ease:cubic-bezier(.4,0,.2,1);
}
*,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
html{scroll-behavior:smooth}
body{background:var(--bg);color:var(--t);font-family:var(--fb);overflow-x:hidden;cursor:none}
::-webkit-scrollbar{width:4px}
::-webkit-scrollbar-track{background:var(--bg2)}
::-webkit-scrollbar-thumb{background:var(--r);border-radius:2px}
::selection{background:var(--r);color:#fff}

/* ── CURSOR ─────────────────────────────────── */
#cur,#cur2{position:fixed;border-radius:50%;pointer-events:none;z-index:99999;transform:translate(-50%,-50%)}
#cur{width:8px;height:8px;background:var(--rb);box-shadow:0 0 10px var(--rg)}
#cur2{width:30px;height:30px;border:1px solid rgba(200,0,26,.45)}

/* ── LOADING ─────────────────────────────────── */
#ld{position:fixed;inset:0;background:var(--bg);z-index:9999;display:flex;align-items:center;justify-content:center;flex-direction:column;gap:18px;transition:opacity .6s,visibility .6s}
#ld.off{opacity:0;visibility:hidden;pointer-events:none}
.ld-logo{width:60px;height:60px;animation:ldp 1.2s ease-in-out infinite}
@keyframes ldp{0%,100%{filter:drop-shadow(0 0 12px var(--r))}50%{filter:drop-shadow(0 0 28px var(--rb))}}
.ld-track{width:150px;height:2px;background:var(--bg3);border-radius:1px;overflow:hidden}
.ld-bar{height:100%;width:0;background:linear-gradient(90deg,var(--rd),var(--rb));box-shadow:0 0 6px var(--r)}
.ld-lbl{font-family:var(--fm);font-size:10px;letter-spacing:3px;color:var(--t3);text-transform:uppercase}

/* ── TOS ─────────────────────────────────────── */
#tos{position:fixed;inset:0;background:rgba(0,0,0,.96);z-index:9000;display:flex;align-items:center;justify-content:center;padding:12px;transition:opacity .5s,visibility .5s;backdrop-filter:blur(4px)}
#tos.off{opacity:0;visibility:hidden;pointer-events:none}
.tm{background:var(--bg2);border:1px solid var(--br);border-radius:20px;max-width:640px;width:100%;max-height:92vh;display:flex;flex-direction:column;overflow:hidden;animation:tma .4s cubic-bezier(.34,1.56,.64,1)}
@keyframes tma{from{opacity:0;transform:scale(.9) translateY(20px)}to{opacity:1;transform:none}}
.tm-top{padding:20px 24px 16px;border-bottom:1px solid var(--b);display:flex;align-items:center;gap:12px;flex-shrink:0;background:linear-gradient(180deg,rgba(200,0,26,.05),transparent)}
.tm-top h2{font-family:var(--fd);font-size:20px;letter-spacing:2px}
.tm-top p{font-family:var(--fm);font-size:10px;color:var(--t3);margin-top:2px}
.tm-body{padding:18px 24px;overflow-y:auto;flex:1;font-size:12.5px;color:var(--t2);line-height:1.8}
.tm-body::-webkit-scrollbar{width:2px}
.tm-body::-webkit-scrollbar-thumb{background:var(--rd)}
.ts{margin-bottom:15px}
.ts h3{font-family:var(--fm);font-size:10px;letter-spacing:2px;text-transform:uppercase;color:var(--rb);margin-bottom:5px;display:flex;align-items:center;gap:6px}
.ts h3::before{content:'';width:2px;height:10px;background:var(--r);display:inline-block;border-radius:1px}
.ts ul{padding-left:14px;margin-top:4px}
.ts ul li{margin-bottom:3px}
.tm-foot{padding:14px 24px 18px;border-top:1px solid var(--b);background:var(--bg3);flex-shrink:0}
.tc-row{display:flex;align-items:center;gap:10px;margin-bottom:12px;cursor:pointer;user-select:none}
.tc-box{width:17px;height:17px;border:1.5px solid var(--br);border-radius:4px;display:flex;align-items:center;justify-content:center;flex-shrink:0;transition:.2s}
.tc-row.on .tc-box{background:var(--r);border-color:var(--r);box-shadow:0 0 8px var(--rg)}
.tc-ck{opacity:0;transform:scale(.3);transition:.2s;width:9px;height:9px}
.tc-row.on .tc-ck{opacity:1;transform:scale(1)}
.tc-lbl{font-size:12px;color:var(--t2)}
.ta-btn{width:100%;padding:13px;background:var(--r);color:#fff;border:none;border-radius:var(--rad);font-family:var(--fd);font-size:17px;letter-spacing:2px;cursor:pointer;transition:.25s var(--ease)}
.ta-btn:not(:disabled):hover{background:var(--rb);box-shadow:0 0 28px var(--rg);transform:translateY(-1px)}
.ta-btn:disabled{opacity:.3;cursor:not-allowed}

/* ── CHANNEL MODAL ───────────────────────────── */
#chan{position:fixed;inset:0;z-index:8000;display:flex;align-items:flex-end;justify-content:center;transition:opacity .35s,visibility .35s}
#chan.off{opacity:0;visibility:hidden;pointer-events:none}
.chan-bg{position:absolute;inset:0;background:rgba(0,0,0,.72);backdrop-filter:blur(8px)}
.chan-box{position:relative;background:var(--bg2);border:1px solid var(--br);border-bottom:none;border-radius:20px 20px 0 0;width:100%;max-width:540px;overflow:hidden;box-shadow:0 -16px 70px rgba(0,0,0,.7);transition:transform .4s cubic-bezier(.34,1.2,.64,1)}
#chan.off .chan-box{transform:translateY(100%)}
.chan-drag{width:32px;height:3px;background:var(--b);border-radius:2px;margin:12px auto 0}
.chan-head{padding:14px 22px 12px;border-bottom:1px solid var(--b);display:flex;align-items:center;justify-content:space-between}
.chan-title{display:flex;align-items:center;gap:10px}
.chan-ico{width:38px;height:38px;background:var(--bg3);border-radius:10px;display:flex;align-items:center;justify-content:center;font-size:20px;border:1px solid var(--b)}
.chan-name{font-family:var(--fd);font-size:21px;letter-spacing:1px;color:var(--t)}
.chan-subt{font-family:var(--fm);font-size:9px;color:var(--t3);letter-spacing:.5px;margin-top:1px}
.chan-cls{width:30px;height:30px;background:var(--bg3);border:1px solid var(--b);border-radius:50%;display:flex;align-items:center;justify-content:center;cursor:pointer;color:var(--t2);transition:.2s;flex-shrink:0}
.chan-cls:hover{border-color:var(--br);color:var(--rb)}
.chan-body{padding:16px 22px 0}
.chan-pills{display:grid;grid-template-columns:1fr 1fr;gap:7px;margin-bottom:14px}
.cpill{background:var(--bg3);border:1px solid var(--b);border-radius:9px;padding:9px 12px;cursor:pointer;transition:.2s;position:relative}
.cpill:hover,.cpill.sel{border-color:var(--br);background:rgba(200,0,26,.06)}
.cpill.sel{border-color:var(--r)}
.cpill-l{font-size:11px;color:var(--t2);display:block;margin-bottom:2px;font-family:var(--fm)}
.cpill-p{font-family:var(--fd);font-size:19px;color:var(--rb)}
.cpill-chk{position:absolute;top:7px;right:7px;width:14px;height:14px;background:var(--r);border-radius:50%;display:flex;align-items:center;justify-content:center;opacity:0;transition:.2s;font-size:9px;color:#fff}
.cpill.sel .cpill-chk{opacity:1}
.chan-steps{display:flex;flex-direction:column;gap:8px;margin-bottom:14px}
.cstep{display:flex;gap:10px;align-items:flex-start}
.cstep-n{width:20px;height:20px;background:var(--rgs);border:1px solid var(--br);border-radius:50%;display:flex;align-items:center;justify-content:center;font-family:var(--fm);font-size:9px;color:var(--rb);flex-shrink:0;margin-top:1px}
.cstep-t strong{display:block;font-size:12.5px;font-weight:600;color:var(--t);margin-bottom:1px}
.cstep-t span{font-size:11px;color:var(--t3)}
.chan-inv{display:flex;align-items:center;background:var(--bg3);border:1px solid var(--b);border-radius:8px;overflow:hidden;margin-bottom:14px}
.chan-inv-u{flex:1;padding:10px 13px;font-family:var(--fm);font-size:12px;color:var(--t2)}
.chan-inv-c{padding:10px 15px;background:var(--rgs);border:none;border-left:1px solid var(--b);color:var(--rb);font-family:var(--fm);font-size:10px;cursor:pointer;transition:.2s;white-space:nowrap;letter-spacing:.5px}
.chan-inv-c:hover{background:var(--r);color:#fff}
.chan-inv-c.ok{background:#0a5c2e;color:#4ade80}
.chan-cta{display:flex;gap:8px;padding-bottom:18px}
.chan-go{flex:1;padding:12px;background:var(--r);color:#fff;border:none;border-radius:var(--rad);font-family:var(--fd);font-size:17px;letter-spacing:2px;cursor:pointer;transition:.25s var(--ease);display:flex;align-items:center;justify-content:center;gap:7px;text-decoration:none}
.chan-go:hover{background:var(--rb);box-shadow:0 0 24px var(--rg);transform:translateY(-1px)}
.chan-alt{padding:12px 14px;background:var(--bg3);border:1px solid var(--b);border-radius:var(--rad);color:var(--t2);font-family:var(--fm);font-size:10px;cursor:pointer;transition:.2s;text-decoration:none;display:flex;align-items:center;justify-content:center;text-align:center;line-height:1.3}
.chan-alt:hover{border-color:var(--br);color:var(--rb)}
.chan-note{font-family:var(--fm);font-size:9.5px;color:var(--t3);text-align:center;margin-top:8px;line-height:1.6;padding-bottom:6px}

/* ── NOTIFICATIONS ───────────────────────────── */
#nc{position:fixed;bottom:18px;left:18px;z-index:7000;display:flex;flex-direction:column;gap:7px;pointer-events:none}
.ncard{background:rgba(10,10,10,.96);border:1px solid rgba(200,0,26,.2);border-radius:11px;padding:9px 13px;display:flex;align-items:center;gap:9px;max-width:230px;backdrop-filter:blur(16px);animation:ncin .3s cubic-bezier(.34,1.56,.64,1);transition:opacity .3s,transform .3s}
.ncard.out{opacity:0;transform:translateX(-14px)}
@keyframes ncin{from{opacity:0;transform:translateX(-14px)}to{opacity:1;transform:none}}
.nav2{width:26px;height:26px;border-radius:50%;background:var(--r);display:flex;align-items:center;justify-content:center;font-family:var(--fd);font-size:12px;flex-shrink:0}
.nct p{font-size:11px;color:var(--t);font-weight:500;line-height:1.3}
.nct span{font-size:10px;color:var(--rb)}
.nct small{font-size:9px;color:var(--t3)}

/* ── NAVBAR ──────────────────────────────────── */
#nav{position:fixed;top:0;left:0;right:0;z-index:6000;padding:0 26px;height:58px;display:flex;align-items:center;justify-content:space-between;transition:background .3s,border .3s,backdrop-filter .3s}
#nav.scr{background:rgba(6,6,6,.9);backdrop-filter:blur(18px);border-bottom:1px solid var(--b)}
.brand{display:flex;align-items:center;gap:7px;text-decoration:none}
.brand-logo{width:28px;height:28px;filter:drop-shadow(0 0 5px var(--r));transition:filter .3s}
.brand:hover .brand-logo{filter:drop-shadow(0 0 12px var(--rb))}
.brand-name{font-family:var(--fd);font-size:20px;letter-spacing:3px;color:var(--t)}
.brand-name b{color:var(--r)}
.navlinks{display:flex;align-items:center;gap:2px;list-style:none}
.navlinks a{color:var(--t3);text-decoration:none;font-size:11px;font-weight:600;padding:5px 11px;border-radius:5px;transition:.2s;letter-spacing:.5px;text-transform:uppercase}
.navlinks a:hover{color:var(--t);background:rgba(255,255,255,.04)}
.nav-r{display:flex;align-items:center;gap:9px}
.obadge{display:flex;align-items:center;gap:5px;padding:4px 10px;background:rgba(0,180,70,.05);border:1px solid rgba(0,180,70,.14);border-radius:20px;font-family:var(--fm);font-size:9px;color:#00c864;letter-spacing:.5px}
.gdot{width:5px;height:5px;background:#00c864;border-radius:50%;animation:pg 2s ease-in-out infinite}
@keyframes pg{0%,100%{box-shadow:0 0 0 0 rgba(0,200,100,.5)}70%{box-shadow:0 0 0 4px transparent}}
.jbtn{display:flex;align-items:center;gap:6px;padding:6px 15px;background:var(--r);color:#fff;text-decoration:none;border-radius:7px;font-family:var(--fd);font-size:13px;letter-spacing:1.5px;transition:.25s;border:none;cursor:pointer}
.jbtn:hover{background:var(--rb);box-shadow:0 0 16px var(--rg);transform:translateY(-1px)}
.ham{display:none;flex-direction:column;gap:4px;cursor:pointer;padding:6px;background:none;border:none}
.ham span{display:block;width:19px;height:2px;background:var(--t);border-radius:1px;transition:.25s}
.ham.open span:nth-child(1){transform:rotate(45deg) translate(4px,4px)}
.ham.open span:nth-child(2){opacity:0}
.ham.open span:nth-child(3){transform:rotate(-45deg) translate(4px,-4px)}
.mmnav{display:none;position:fixed;top:58px;left:0;right:0;background:rgba(6,6,6,.98);backdrop-filter:blur(18px);border-bottom:1px solid var(--b);padding:10px 18px 16px;flex-direction:column;gap:2px;z-index:5999}
.mmnav.open{display:flex}
.mmnav a{color:var(--t2);text-decoration:none;font-size:13px;font-weight:600;padding:10px 12px;border-radius:7px;transition:.2s;text-transform:uppercase;letter-spacing:.5px}
.mmnav a:hover{color:var(--t);background:rgba(255,255,255,.04)}
#sb{position:fixed;top:66px;right:15px;z-index:6001;width:32px;height:32px;background:var(--bg3);border:1px solid var(--b);border-radius:50%;display:flex;align-items:center;justify-content:center;cursor:pointer;transition:.2s;color:var(--t3)}
#sb:hover{border-color:var(--br);color:var(--rb)}

/* ── HERO ────────────────────────────────────── */
#hero{min-height:100vh;display:flex;align-items:center;justify-content:center;position:relative;overflow:hidden;padding:84px 22px 48px}
.hgrid{position:absolute;inset:0;background-image:linear-gradient(rgba(200,0,26,.03) 1px,transparent 1px),linear-gradient(90deg,rgba(200,0,26,.03) 1px,transparent 1px);background-size:46px 46px;animation:gm 18s linear infinite;mask-image:radial-gradient(ellipse 80% 80% at 50% 50%,black 30%,transparent 100%)}
@keyframes gm{0%{background-position:0 0}100%{background-position:46px 46px}}
.scanlines{position:absolute;inset:0;background:repeating-linear-gradient(0deg,transparent,transparent 2px,rgba(0,0,0,.03) 2px,rgba(0,0,0,.03) 4px);pointer-events:none;z-index:1}
.hglow{position:absolute;width:650px;height:650px;background:radial-gradient(circle,rgba(200,0,26,.08) 0%,transparent 65%);top:50%;left:50%;transform:translate(-50%,-50%);pointer-events:none;animation:hgp 4s ease-in-out infinite}
@keyframes hgp{0%,100%{opacity:.8;transform:translate(-50%,-50%) scale(1)}50%{opacity:1;transform:translate(-50%,-50%) scale(1.07)}}
.hglow2{position:absolute;width:280px;height:280px;background:radial-gradient(circle,rgba(200,0,26,.05) 0%,transparent 70%);top:18%;right:9%;animation:hg2 6s ease-in-out infinite;pointer-events:none}
@keyframes hg2{0%,100%{transform:translateY(0)}50%{transform:translateY(-22px)}}
.hc{text-align:center;position:relative;z-index:2;max-width:800px;width:100%}
.hero-ey{display:inline-flex;align-items:center;gap:7px;padding:4px 13px 4px 7px;background:rgba(200,0,26,.07);border:1px solid rgba(200,0,26,.2);border-radius:20px;margin-bottom:20px;animation:fu .7s .15s both}
.ey-tag{padding:2px 8px;background:var(--r);border-radius:11px;font-family:var(--fm);font-size:8px;letter-spacing:1px;text-transform:uppercase;color:#fff}
.ey-txt{font-family:var(--fm);font-size:9.5px;color:var(--rb);letter-spacing:1px}
.htitle{font-family:var(--fd);font-size:clamp(50px,8vw,96px);line-height:.94;letter-spacing:2px;margin-bottom:16px;animation:fu .7s .3s both}
.htitle em{font-style:normal;color:var(--r);display:block}
.hsub{font-size:14px;color:var(--t2);max-width:480px;margin:0 auto 32px;line-height:1.7;animation:fu .7s .45s both}
@keyframes fu{from{opacity:0;transform:translateY(18px)}to{opacity:1;transform:none}}
.hbtns{display:flex;gap:11px;justify-content:center;flex-wrap:wrap;animation:fu .7s .6s both}
.stat-rib{display:grid;grid-template-columns:repeat(4,1fr);gap:1px;background:var(--b);margin-top:54px;overflow:hidden;border-radius:12px;animation:fu .7s .75s both}
.sc{background:var(--bg2);padding:16px 10px;text-align:center}
.sn{font-family:var(--fd);font-size:28px;letter-spacing:1px;line-height:1}
.sn b{color:var(--r)}
.sl{font-family:var(--fm);font-size:8px;color:var(--t3);letter-spacing:2px;text-transform:uppercase;margin-top:4px}

/* ── SECTIONS ────────────────────────────────── */
section{padding:84px 22px;position:relative;z-index:1}
.mxc{max-width:1120px;margin:0 auto}
.slbl{font-family:var(--fm);font-size:10px;letter-spacing:3px;text-transform:uppercase;color:var(--r);margin-bottom:8px;display:block}
.stit{font-family:var(--fd);font-size:clamp(30px,5vw,52px);letter-spacing:2px;line-height:1;margin-bottom:10px}
.ssub{font-size:13.5px;color:var(--t2);max-width:480px;line-height:1.7}
.tc{text-align:center}
.tc .ssub{margin:0 auto}
.rv{opacity:0;transform:translateY(22px);transition:opacity .6s var(--ease),transform .6s var(--ease)}
.rv.vis{opacity:1;transform:none}

/* ── MARQUEE ─────────────────────────────────── */
.mq-wrap{background:var(--bg2);border-top:1px solid var(--b);border-bottom:1px solid var(--b);padding:12px 0;overflow:hidden}
.mq{display:flex;animation:mqa 24s linear infinite;width:max-content}
.mqi{display:flex;align-items:center;gap:7px;padding:0 28px;border-right:1px solid var(--b);font-family:var(--fd);font-size:14px;letter-spacing:2px;color:var(--t3);white-space:nowrap}
.mqi b{color:var(--r)}
@keyframes mqa{0%{transform:translateX(0)}100%{transform:translateX(-50%)}}

/* ── SHOP CONTROLS ───────────────────────────── */
.shop-top{display:flex;align-items:center;justify-content:space-between;gap:14px;flex-wrap:wrap;margin-bottom:22px}
.srch-wrap{position:relative}
.srch-ico{position:absolute;left:11px;top:50%;transform:translateY(-50%);pointer-events:none;color:var(--t3)}
.srch{background:var(--bg2);border:1px solid var(--b);border-radius:7px;padding:8px 11px 8px 35px;color:var(--t);font-family:var(--fm);font-size:12px;outline:none;width:200px;transition:.2s}
.srch::placeholder{color:var(--t3)}
.srch:focus{border-color:var(--br);box-shadow:0 0 7px var(--rgs)}
.cat-tabs{display:flex;gap:5px;flex-wrap:wrap}
.ctab{padding:6px 14px;background:var(--bg2);border:1px solid var(--b);border-radius:6px;color:var(--t3);font-family:var(--fm);font-size:10px;font-weight:500;cursor:pointer;transition:.2s;letter-spacing:.5px;text-transform:uppercase}
.ctab.on,.ctab:hover{background:var(--rgs);border-color:var(--br);color:var(--rb)}

/* ── PRODUCT GRID ────────────────────────────── */
.pgrid{display:grid;grid-template-columns:repeat(auto-fill,minmax(255px,1fr));gap:14px}

/* ── PRODUCT CARD ────────────────────────────── */
.pcard{background:var(--bg2);border:1px solid var(--b);border-radius:var(--rad2);overflow:hidden;position:relative;display:flex;flex-direction:column;transition:border-color .3s,box-shadow .3s,transform .3s var(--ease)}
.pcard:hover{border-color:var(--br);box-shadow:0 0 35px rgba(200,0,26,.09),0 18px 50px rgba(0,0,0,.4);transform:translateY(-5px)}
.pcard::before{content:'';position:absolute;top:0;left:0;right:0;height:2px;background:linear-gradient(90deg,transparent,var(--r),transparent);opacity:0;transition:opacity .3s}
.pcard:hover::before{opacity:1}
.pc-top{padding:18px 18px 14px;display:flex;align-items:flex-start;justify-content:space-between;gap:10px}
.pc-ico{width:44px;height:44px;background:var(--bg3);border-radius:11px;display:flex;align-items:center;justify-content:center;font-size:21px;border:1px solid var(--b);flex-shrink:0;transition:.25s}
.pcard:hover .pc-ico{border-color:var(--br);box-shadow:0 0 12px var(--rgs)}
.pbadge{padding:3px 8px;border-radius:20px;font-family:var(--fm);font-size:8.5px;letter-spacing:1px;text-transform:uppercase;flex-shrink:0}
.bh{background:rgba(200,0,26,.13);border:1px solid rgba(200,0,26,.28);color:var(--rb)}
.bn{background:rgba(0,160,80,.09);border:1px solid rgba(0,160,80,.22);color:#22c55e}
.bb{background:rgba(200,120,0,.09);border:1px solid rgba(200,120,0,.22);color:#f59e0b}
.pc-body{padding:0 18px 14px;flex:1}
.pc-name{font-family:var(--fd);font-size:19px;letter-spacing:.8px;margin-bottom:2px;color:var(--t)}
.pc-sub{font-family:var(--fm);font-size:9.5px;color:var(--t3);letter-spacing:.3px;margin-bottom:12px}
.prows{display:flex;flex-direction:column;gap:4px}
.prow{display:flex;align-items:center;justify-content:space-between;padding:5px 9px;background:var(--bg3);border-radius:6px;border:1px solid transparent;transition:.2s}
.prow:hover{border-color:var(--b)}
.prow-l{font-family:var(--fm);font-size:10.5px;color:var(--t2)}
.prow-p{font-family:var(--fd);font-size:15px;color:var(--rb)}
.pc-price-big{font-family:var(--fd);font-size:30px;color:var(--rb);line-height:1;margin-bottom:3px}
.pc-price-was{font-family:var(--fm);font-size:10.5px;color:var(--t3)}
.pc-foot{padding:0 18px 18px;margin-top:auto}
.pc-buybtn{width:100%;padding:10px 14px;background:var(--rgs);border:1px solid var(--br);border-radius:7px;color:var(--rb);font-family:var(--fd);font-size:14px;letter-spacing:1.5px;cursor:pointer;transition:.25s var(--ease);display:flex;align-items:center;justify-content:center;gap:7px;position:relative;overflow:hidden}
.pc-buybtn::before{content:'';position:absolute;inset:0;background:var(--r);transform:scaleX(0);transform-origin:left;transition:transform .3s var(--ease)}
.pc-buybtn:hover{color:#fff;border-color:var(--r);box-shadow:0 0 18px var(--rg)}
.pc-buybtn:hover::before{transform:scaleX(1)}
.pc-buybtn .bi{position:relative;z-index:1;display:flex;align-items:center;gap:7px}

/* ── FEATURES ────────────────────────────────── */
#feats{background:var(--bg2);border-top:1px solid var(--b);border-bottom:1px solid var(--b)}
.fg{display:grid;grid-template-columns:repeat(auto-fill,minmax(200px,1fr));gap:12px;margin-top:44px}
.feat{background:var(--bg3);border:1px solid var(--b);border-radius:var(--rad2);padding:22px;transition:.25s var(--ease);position:relative;overflow:hidden}
.feat::after{content:'';position:absolute;bottom:0;left:0;right:0;height:1px;background:linear-gradient(90deg,transparent,var(--r),transparent);opacity:0;transition:opacity .3s}
.feat:hover{border-color:var(--br);transform:translateY(-3px)}
.feat:hover::after{opacity:1}
.feat-ic{width:36px;height:36px;background:var(--rgs);border-radius:8px;display:flex;align-items:center;justify-content:center;color:var(--r);margin-bottom:12px}
.feat-t{font-family:var(--fd);font-size:17px;margin-bottom:5px}
.feat-d{font-size:12px;color:var(--t3);line-height:1.65}

/* ── REVIEWS ─────────────────────────────────── */
.rg{display:grid;grid-template-columns:repeat(auto-fill,minmax(250px,1fr));gap:12px;margin-top:44px}
.rcard{background:var(--bg2);border:1px solid var(--b);border-radius:var(--rad2);padding:20px;transition:.25s;position:relative;overflow:hidden}
.rcard::before{content:'"';position:absolute;top:-14px;right:12px;font-size:95px;line-height:1;font-family:serif;color:var(--r);opacity:.04}
.rcard:hover{border-color:var(--br);transform:translateY(-3px)}
.stars{color:var(--r);font-size:11px;margin-bottom:9px;letter-spacing:2px}
.rev-t{font-size:12.5px;color:var(--t2);line-height:1.7;margin-bottom:14px}
.rev-a{display:flex;align-items:center;gap:8px}
.rev-av{width:30px;height:30px;border-radius:50%;background:var(--r);display:flex;align-items:center;justify-content:center;font-family:var(--fd);font-size:13px;flex-shrink:0}
.rev-n{font-size:12.5px;font-weight:600;color:var(--t)}
.rev-i{font-family:var(--fm);font-size:9px;color:var(--t3)}

/* ── FAQ ─────────────────────────────────────── */
.faq-list{margin-top:42px;max-width:680px;margin-left:auto;margin-right:auto}
.fi2{border-bottom:1px solid var(--b);overflow:hidden}
.faq-q{display:flex;align-items:center;justify-content:space-between;padding:16px 0;cursor:pointer;font-family:var(--fb);font-size:13.5px;font-weight:600;color:var(--t);gap:12px;transition:color .2s}
.faq-q:hover{color:var(--rb)}
.faq-ic{width:18px;height:18px;flex-shrink:0;border-radius:50%;border:1px solid var(--b);display:flex;align-items:center;justify-content:center;color:var(--t3);transition:.25s}
.fi2.open .faq-ic{border-color:var(--r);color:var(--rb);transform:rotate(45deg)}
.faq-a{max-height:0;overflow:hidden;transition:max-height .4s var(--ease),padding .3s;font-size:13px;color:var(--t3);line-height:1.75}
.fi2.open .faq-a{max-height:200px;padding-bottom:13px}

/* ── DISCORD CTA ─────────────────────────────── */
#dcta{background:var(--bg2);border-top:1px solid var(--b);text-align:center}
.dbox{max-width:540px;margin:0 auto;background:var(--bg3);border:1px solid var(--br);border-radius:20px;padding:44px 30px;position:relative;overflow:hidden;box-shadow:0 0 55px rgba(200,0,26,.07)}
.dbox::before{content:'';position:absolute;top:-50%;left:-10%;width:120%;height:120%;background:radial-gradient(ellipse,rgba(200,0,26,.045),transparent 70%);pointer-events:none}
.dinv{display:flex;align-items:center;background:var(--bg2);border:1px solid var(--b);border-radius:8px;overflow:hidden;margin:22px 0 18px}
.dinv-l{flex:1;padding:10px 13px;font-family:var(--fm);font-size:12.5px;color:var(--t2)}
.dinv-c{padding:10px 15px;background:var(--rgs);border:none;border-left:1px solid var(--b);color:var(--rb);font-family:var(--fm);font-size:10px;cursor:pointer;transition:.2s;white-space:nowrap}
.dinv-c:hover{background:var(--r);color:#fff}
.dinv-c.ok{background:#0a5c2e;color:#4ade80}

/* ── FOOTER ──────────────────────────────────── */
footer{background:var(--bg2);border-top:1px solid var(--b);padding:44px 22px 22px}
.fg2{display:grid;grid-template-columns:2fr 1fr 1fr 1fr;gap:30px;max-width:1120px;margin:0 auto 28px}
.fb p{font-size:12px;color:var(--t3);margin-top:9px;line-height:1.65;max-width:210px;font-family:var(--fm)}
.fc2 h4{font-family:var(--fm);font-size:9.5px;letter-spacing:2px;text-transform:uppercase;color:var(--t3);margin-bottom:12px}
.fc2 ul{list-style:none}
.fc2 ul li{margin-bottom:7px}
.fc2 ul li a{font-family:var(--fm);font-size:11px;color:var(--t3);text-decoration:none;transition:color .2s}
.fc2 ul li a:hover{color:var(--rb)}
.fbot{max-width:1120px;margin:0 auto;padding-top:18px;border-top:1px solid var(--b);display:flex;align-items:center;justify-content:space-between;gap:10px;flex-wrap:wrap}
.fbot p{font-family:var(--fm);font-size:10.5px;color:var(--t3)}
.disc-n{font-family:var(--fm);font-size:9.5px;color:var(--t3);text-align:center;max-width:640px;margin:12px auto 0;line-height:1.7}
#fdisc{position:fixed;bottom:18px;right:18px;z-index:6001;width:46px;height:46px;background:var(--r);border-radius:50%;display:flex;align-items:center;justify-content:center;cursor:pointer;box-shadow:0 0 18px var(--rg),0 6px 24px rgba(0,0,0,.4);transition:.25s;text-decoration:none}
#fdisc:hover{transform:scale(1.12);box-shadow:0 0 30px var(--rg)}

/* ── BUTTONS ─────────────────────────────────── */
.btn-p{display:inline-flex;align-items:center;gap:8px;padding:11px 24px;background:var(--r);color:#fff;text-decoration:none;border-radius:var(--rad);font-family:var(--fd);font-size:15px;letter-spacing:1.5px;transition:.25s var(--ease);border:none;cursor:pointer}
.btn-p:hover{background:var(--rb);box-shadow:0 0 28px var(--rg);transform:translateY(-2px)}
.btn-g{display:inline-flex;align-items:center;gap:8px;padding:11px 24px;background:transparent;color:var(--t);text-decoration:none;border-radius:var(--rad);border:1px solid var(--b);font-family:var(--fd);font-size:15px;letter-spacing:1.5px;transition:.25s var(--ease);cursor:pointer}
.btn-g:hover{border-color:var(--br);color:var(--rb);background:var(--rgs);transform:translateY(-2px)}

/* ── RESPONSIVE ──────────────────────────────── */
@media(max-width:1024px){section{padding:64px 18px}}
@media(max-width:768px){
  #nav{padding:0 14px}
  .navlinks,.obadge,.jbtn{display:none}
  .ham{display:flex}
  section{padding:50px 14px}
  .stat-rib{grid-template-columns:repeat(2,1fr)}
  .fg2{grid-template-columns:1fr 1fr}
  #cur,#cur2{display:none}
}
@media(max-width:520px){
  .hbtns{flex-direction:column;align-items:stretch}
  .btn-p,.btn-g{justify-content:center}
  .chan-pills{grid-template-columns:1fr}
  .fg2{grid-template-columns:1fr}
}
</style>
</head>
<body>

<!-- Cursor -->
<div id="cur"></div>
<div id="cur2"></div>

<!-- Loading -->
<div id="ld">
  <svg class="ld-logo" viewBox="0 0 100 100" fill="none">
    <rect width="100" height="100" rx="20" fill="#111"/>
    <path d="M22 75V25H52C62 25 70 33 70 43C70 50 66 56 60 59L72 75H58L47 61H36V75H22ZM36 49H50C54 49 57 46 57 42C57 38 54 35 50 35H36V49Z" fill="#c8001a"/>
    <path d="M60 59L72 75H58" fill="#7a000f"/>
  </svg>
  <div class="ld-track"><div class="ld-bar" id="ldb"></div></div>
  <p class="ld-lbl">Loading Retro Hub</p>
</div>

<!-- TOS Modal -->
<div id="tos">
  <div class="tm">
    <div class="tm-top">
      <svg width="34" height="34" viewBox="0 0 100 100" fill="none" style="flex-shrink:0;filter:drop-shadow(0 0 7px #c8001a)">
        <rect width="100" height="100" rx="16" fill="#111"/>
        <path d="M22 75V25H52C62 25 70 33 70 43C70 50 66 56 60 59L72 75H58L47 61H36V75H22ZM36 49H50C54 49 57 46 57 42C57 38 54 35 50 35H36V49Z" fill="#c8001a"/>
        <path d="M60 59L72 75H58" fill="#7a000f"/>
      </svg>
      <div>
        <h2>TERMS OF SERVICE</h2>
        <p>RETRO HUB &middot; JAN 2025 &middot; READ FULLY BEFORE PROCEEDING</p>
      </div>
    </div>
    <div class="tm-body">
      <div class="ts"><h3>Age Requirement</h3><p>You must be at least <strong>18 years old</strong> to purchase from Retro Hub. By proceeding you confirm this.</p></div>
      <div class="ts"><h3>All Sales Are Final</h3><p>Every purchase is <strong>final and non-refundable</strong>. Once a product is delivered no refund will be issued for any reason including change of mind, inability to use, or third-party service changes.</p></div>
      <div class="ts"><h3>No Affiliation With Third-Party Brands</h3><p>Retro Hub is <strong>not affiliated with</strong> Discord, Spotify, Netflix, Roblox, Crunchyroll, Instagram, TikTok, or Twitch. We are an independent reseller. Products may stop working due to third-party platform changes.</p></div>
      <div class="ts"><h3>User Responsibility</h3><p>You must <strong>not share, resell, leak, or abuse</strong> any delivered product. Violations result in immediate permanent blacklisting.</p></div>
      <div class="ts"><h3>Chargebacks = Permanent Ban</h3><p>Any chargeback or payment reversal after delivery constitutes <strong>fraud</strong>. The user will be permanently blacklisted and the incident may be reported to payment processors.</p></div>
      <div class="ts"><h3>Right to Refuse Service</h3><p>Staff hold the absolute right to refuse service, revoke access, or permanently ban any user for violations. No refund issued upon ban.</p></div>
      <div class="ts"><h3>Services Provided As-Is</h3><p>All products are provided <strong>as-is without warranty</strong>. We do not guarantee uninterrupted access or specific service duration after delivery.</p></div>
      <div class="ts"><h3>Liability Limitation</h3><p>To the maximum extent permitted by law, Retro Hub and its staff are not liable for any damages arising from use or inability to use our products.</p></div>
      <div class="ts"><h3>Governing Law</h3><p>These Terms are governed by applicable international digital commerce law. Disputes resolved by good-faith negotiation, then binding arbitration if unresolved.</p></div>
    </div>
    <div class="tm-foot">
      <label class="tc-row" id="tcrow">
        <div class="tc-box">
          <svg class="tc-ck" viewBox="0 0 9 9" fill="none" stroke="white" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
            <path d="M1 4.5L3.5 7L8 1.5"/>
          </svg>
        </div>
        <span class="tc-lbl">I have fully read and agree to the Terms of Service. I am 18+ years of age.</span>
      </label>
      <button class="ta-btn" id="ta" disabled>I AGREE &amp; ENTER RETRO HUB</button>
    </div>
  </div>
</div>

<!-- Channel Purchase Modal -->
<div id="chan" class="off">
  <div class="chan-bg" id="chan-bg"></div>
  <div class="chan-box">
    <div class="chan-drag"></div>
    <div class="chan-head">
      <div class="chan-title">
        <div class="chan-ico" id="chan-ico">💜</div>
        <div>
          <div class="chan-name" id="chan-name">Product</div>
          <div class="chan-subt" id="chan-subt">RETRO HUB &middot; INSTANT DELIVERY</div>
        </div>
      </div>
      <div class="chan-cls" id="chan-cls">
        <svg width="13" height="13" viewBox="0 0 13 13" fill="none" stroke="currentColor" stroke-width="2">
          <path d="M1 1l11 11M12 1L1 12"/>
        </svg>
      </div>
    </div>
    <div class="chan-body">
      <div class="chan-pills" id="chan-pills"></div>
      <div class="chan-steps">
        <div class="cstep"><div class="cstep-n">1</div><div class="cstep-t"><strong>Select your tier above</strong><span>Tap the option you want to purchase</span></div></div>
        <div class="cstep"><div class="cstep-n">2</div><div class="cstep-t"><strong>Open the product channel</strong><span>Click the button or copy the invite link below</span></div></div>
        <div class="cstep"><div class="cstep-n">3</div><div class="cstep-t"><strong>Open a ticket or DM staff</strong><span>Tell them your tier, pay, and you are done!</span></div></div>
      </div>
      <div class="chan-inv">
        <span class="chan-inv-u" id="chan-url">discord.gg/DfU3ZQNgAV</span>
        <button class="chan-inv-c" id="chan-cpy">COPY</button>
      </div>
      <div class="chan-cta">
        <a class="chan-go" id="chan-go" href="#" target="_blank" rel="noopener">
          <svg width="14" height="14" viewBox="0 0 24 24" fill="currentColor">
            <path d="M20.317 4.37a19.791 19.791 0 0 0-4.885-1.515.074.074 0 0 0-.079.037c-.21.375-.444.864-.608 1.25a18.27 18.27 0 0 0-5.487 0 12.64 12.64 0 0 0-.617-1.25.077.077 0 0 0-.079-.037A19.736 19.736 0 0 0 3.677 4.37a.07.07 0 0 0-.032.027C.533 9.046-.32 13.58.099 18.057.1 18.08.114 18.1.135 18.115a19.9 19.9 0 0 0 5.993 3.03.078.078 0 0 0 .084-.028c.462-.63.874-1.295 1.226-1.994a.076.076 0 0 0-.041-.106 13.107 13.107 0 0 1-1.872-.892.077.077 0 0 1-.008-.128 10.2 10.2 0 0 0 .372-.292.074.074 0 0 1 .077-.01c3.928 1.793 8.18 1.793 12.062 0a.074.074 0 0 1 .078.01c.12.098.246.198.373.292a.077.077 0 0 1-.006.127 12.299 12.299 0 0 1-1.873.892.077.077 0 0 0-.041.107c.36.698.772 1.362 1.225 1.993a.076.076 0 0 0 .084.028 19.839 19.839 0 0 0 6.002-3.03.077.077 0 0 0 .032-.054c.5-5.177-.838-9.674-3.549-13.66a.061.061 0 0 0-.031-.03z"/>
          </svg>
          OPEN CHANNEL
        </a>
        <a class="chan-alt" href="https://discord.gg/DfU3ZQNgAV" target="_blank" rel="noopener">Main<br/>Server</a>
      </div>
      <p class="chan-note">All sales final &middot; No refunds &middot; By purchasing you agree to our ToS &middot; Not affiliated with any platform</p>
    </div>
  </div>
</div>

<!-- Notifications -->
<div id="nc"></div>

<!-- Navbar -->
<nav id="nav">
  <a href="#" class="brand">
    <svg class="brand-logo" viewBox="0 0 100 100" fill="none">
      <path d="M22 75V25H52C62 25 70 33 70 43C70 50 66 56 60 59L72 75H58L47 61H36V75H22ZM36 49H50C54 49 57 46 57 42C57 38 54 35 50 35H36V49Z" fill="#c8001a"/>
      <path d="M60 59L72 75H58" fill="#7a000f"/>
    </svg>
    <span class="brand-name">RETRO <b>HUB</b></span>
  </a>
  <ul class="navlinks">
    <li><a href="#shop">Shop</a></li>
    <li><a href="#feats">Features</a></li>
    <li><a href="#reviews">Reviews</a></li>
    <li><a href="#faq">FAQ</a></li>
  </ul>
  <div class="nav-r">
    <div class="obadge"><div class="gdot"></div>ONLINE</div>
    <a href="https://discord.gg/DfU3ZQNgAV" target="_blank" rel="noopener" class="jbtn">
      <svg width="13" height="13" viewBox="0 0 24 24" fill="currentColor">
        <path d="M20.317 4.37a19.791 19.791 0 0 0-4.885-1.515.074.074 0 0 0-.079.037c-.21.375-.444.864-.608 1.25a18.27 18.27 0 0 0-5.487 0 12.64 12.64 0 0 0-.617-1.25.077.077 0 0 0-.079-.037A19.736 19.736 0 0 0 3.677 4.37a.07.07 0 0 0-.032.027C.533 9.046-.32 13.58.099 18.057.1 18.08.114 18.1.135 18.115a19.9 19.9 0 0 0 5.993 3.03.078.078 0 0 0 .084-.028c.462-.63.874-1.295 1.226-1.994a.076.076 0 0 0-.041-.106 13.107 13.107 0 0 1-1.872-.892.077.077 0 0 1-.008-.128 10.2 10.2 0 0 0 .372-.292.074.074 0 0 1 .077-.01c3.928 1.793 8.18 1.793 12.062 0a.074.074 0 0 1 .078.01c.12.098.246.198.373.292a.077.077 0 0 1-.006.127 12.299 12.299 0 0 1-1.873.892.077.077 0 0 0-.041.107c.36.698.772 1.362 1.225 1.993a.076.076 0 0 0 .084.028 19.839 19.839 0 0 0 6.002-3.03.077.077 0 0 0 .032-.054c.5-5.177-.838-9.674-3.549-13.66a.061.061 0 0 0-.031-.03z"/>
      </svg>
      JOIN DISCORD
    </a>
    <button class="ham" id="ham"><span></span><span></span><span></span></button>
  </div>
</nav>

<div class="mmnav" id="mmnav">
  <a href="#shop">Shop</a>
  <a href="#feats">Features</a>
  <a href="#reviews">Reviews</a>
  <a href="#faq">FAQ</a>
  <a href="https://discord.gg/DfU3ZQNgAV" target="_blank" rel="noopener" style="color:var(--rb)">Join Discord</a>
</div>

<button id="sb" title="Sound">
  <svg id="son" width="13" height="13" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polygon points="11 5 6 9 2 9 2 15 6 15 11 19 11 5"/><path d="M19.07 4.93a10 10 0 0 1 0 14.14M15.54 8.46a5 5 0 0 1 0 7.07"/></svg>
  <svg id="soff" width="13" height="13" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" style="display:none"><polygon points="11 5 6 9 2 9 2 15 6 15 11 19 11 5"/><line x1="23" y1="9" x2="17" y2="15"/><line x1="17" y1="9" x2="23" y2="15"/></svg>
</button>

<!-- Hero -->
<section id="hero">
  <div class="hgrid"></div>
  <div class="scanlines"></div>
  <div class="hglow"></div>
  <div class="hglow2"></div>
  <div class="hc">
    <div class="hero-ey">
      <span class="ey-tag">LIVE</span>
      <span class="ey-txt">DELIVERY ACTIVE &middot; ALL CHANNELS OPEN</span>
    </div>
    <h1 class="htitle">PREMIUM<br/><em>DIGITAL</em>SERVICES</h1>
    <p class="hsub">Nitro &middot; Decos &middot; Netflix &middot; Robux &middot; Crunchyroll &middot; Followers &amp; more &mdash; at prices nobody else offers.</p>
    <div class="hbtns">
      <a href="#shop" class="btn-p">
        <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5"><circle cx="9" cy="21" r="1"/><circle cx="20" cy="21" r="1"/><path d="M1 1h4l2.68 13.39a2 2 0 0 0 2 1.61h9.72a2 2 0 0 0 2-1.61L23 6H6"/></svg>
        Browse Shop
      </a>
      <a href="https://discord.gg/DfU3ZQNgAV" target="_blank" rel="noopener" class="btn-g">
        <svg width="14" height="14" viewBox="0 0 24 24" fill="currentColor"><path d="M20.317 4.37a19.791 19.791 0 0 0-4.885-1.515.074.074 0 0 0-.079.037c-.21.375-.444.864-.608 1.25a18.27 18.27 0 0 0-5.487 0 12.64 12.64 0 0 0-.617-1.25.077.077 0 0 0-.079-.037A19.736 19.736 0 0 0 3.677 4.37a.07.07 0 0 0-.032.027C.533 9.046-.32 13.58.099 18.057.1 18.08.114 18.1.135 18.115a19.9 19.9 0 0 0 5.993 3.03.078.078 0 0 0 .084-.028c.462-.63.874-1.295 1.226-1.994a.076.076 0 0 0-.041-.106 13.107 13.107 0 0 1-1.872-.892.077.077 0 0 1-.008-.128 10.2 10.2 0 0 0 .372-.292.074.074 0 0 1 .077-.01c3.928 1.793 8.18 1.793 12.062 0a.074.074 0 0 1 .078.01c.12.098.246.198.373.292a.077.077 0 0 1-.006.127 12.299 12.299 0 0 1-1.873.892.077.077 0 0 0-.041.107c.36.698.772 1.362 1.225 1.993a.076.076 0 0 0 .084.028 19.839 19.839 0 0 0 6.002-3.03.077.077 0 0 0 .032-.054c.5-5.177-.838-9.674-3.549-13.66a.061.061 0 0 0-.031-.03z"/></svg>
        Join Server
      </a>
    </div>
    <div class="stat-rib">
      <div class="sc"><div class="sn"><span class="ctr" data-t="100">0</span><b>+</b></div><div class="sl">Members</div></div>
      <div class="sc"><div class="sn"><span class="ctr" data-t="15">0</span><b>+</b></div><div class="sl">Orders Done</div></div>
      <div class="sc"><div class="sn"><span class="ctr" data-t="9">0</span></div><div class="sl">Categories</div></div>
      <div class="sc"><div class="sn"><span class="ctr" data-t="99">0</span><b>%</b></div><div class="sl">Uptime</div></div>
    </div>
  </div>
</section>

<!-- Marquee -->
<div class="mq-wrap">
  <div class="mq">
    <div class="mqi"><b>&#9679;</b>&nbsp;DISCORD NITRO</div><div class="mqi"><b>&#9679;</b>&nbsp;SPOTIFY PREMIUM</div>
    <div class="mqi"><b>&#9679;</b>&nbsp;NETFLIX LIFETIME</div><div class="mqi"><b>&#9679;</b>&nbsp;ROBUX ACCOUNTS</div>
    <div class="mqi"><b>&#9679;</b>&nbsp;CRUNCHYROLL</div><div class="mqi"><b>&#9679;</b>&nbsp;DISCORD DECOS</div>
    <div class="mqi"><b>&#9679;</b>&nbsp;AGED ACCOUNTS</div><div class="mqi"><b>&#9679;</b>&nbsp;BOTTED MEMBERS</div>
    <div class="mqi"><b>&#9679;</b>&nbsp;CRYPTO FLASHER</div><div class="mqi"><b>&#9679;</b>&nbsp;INSTAGRAM FOLLOWERS</div>
    <div class="mqi"><b>&#9679;</b>&nbsp;TIKTOK FOLLOWERS</div><div class="mqi"><b>&#9679;</b>&nbsp;TWITCH ACCOUNTS</div>
    <div class="mqi"><b>&#9679;</b>&nbsp;DISCORD NITRO</div><div class="mqi"><b>&#9679;</b>&nbsp;SPOTIFY PREMIUM</div>
    <div class="mqi"><b>&#9679;</b>&nbsp;NETFLIX LIFETIME</div><div class="mqi"><b>&#9679;</b>&nbsp;ROBUX ACCOUNTS</div>
    <div class="mqi"><b>&#9679;</b>&nbsp;CRUNCHYROLL</div><div class="mqi"><b>&#9679;</b>&nbsp;DISCORD DECOS</div>
    <div class="mqi"><b>&#9679;</b>&nbsp;AGED ACCOUNTS</div><div class="mqi"><b>&#9679;</b>&nbsp;BOTTED MEMBERS</div>
    <div class="mqi"><b>&#9679;</b>&nbsp;CRYPTO FLASHER</div><div class="mqi"><b>&#9679;</b>&nbsp;INSTAGRAM FOLLOWERS</div>
    <div class="mqi"><b>&#9679;</b>&nbsp;TIKTOK FOLLOWERS</div><div class="mqi"><b>&#9679;</b>&nbsp;TWITCH ACCOUNTS</div>
  </div>
</div>

<!-- Shop -->
<section id="shop">
  <div class="mxc">
    <div class="tc rv">
      <span class="slbl">Digital Storefront</span>
      <h2 class="stit">All Products</h2>
      <p class="ssub">Click any card &mdash; a panel opens with pricing, steps, and a direct channel link.</p>
    </div>
    <div class="shop-top rv" style="margin-top:32px">
      <div class="srch-wrap">
        <svg class="srch-ico" width="13" height="13" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="11" cy="11" r="8"/><path d="m21 21-4.35-4.35"/></svg>
        <input class="srch" id="si" type="text" placeholder="Search products..."/>
      </div>
      <div class="cat-tabs" id="ctabs">
        <button class="ctab on" data-cat="all">All</button>
        <button class="ctab" data-cat="discord">Discord</button>
        <button class="ctab" data-cat="streaming">Streaming</button>
        <button class="ctab" data-cat="gaming">Gaming</button>
        <button class="ctab" data-cat="social">Social</button>
        <button class="ctab" data-cat="crypto">Crypto</button>
      </div>
    </div>
    <div class="pgrid" id="pgrid"></div>
  </div>
</section>

<!-- Features -->
<section id="feats">
  <div class="mxc">
    <div class="tc rv">
      <span class="slbl">Why Retro Hub</span>
      <h2 class="stit">Built Different</h2>
      <p class="ssub">A growing community-backed shop with real prices and real support.</p>
    </div>
    <div class="fg">
      <div class="feat rv"><div class="feat-ic"><svg width="17" height="17" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M13 2L3 14h9l-1 8 10-12h-9l1-8z"/></svg></div><div class="feat-t">Instant Delivery</div><div class="feat-d">Most products reach your DMs within minutes of payment, around the clock.</div></div>
      <div class="feat rv"><div class="feat-ic"><svg width="17" height="17" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg></div><div class="feat-t">Verified Stock</div><div class="feat-d">Every product tested before listing. Dead on arrival? We replace it, no hassle.</div></div>
      <div class="feat rv"><div class="feat-ic"><svg width="17" height="17" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg></div><div class="feat-t">Fast Support</div><div class="feat-d">Real staff respond to tickets in minutes. No bots, no waiting days.</div></div>
      <div class="feat rv"><div class="feat-ic"><svg width="17" height="17" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="12" y1="1" x2="12" y2="23"/><path d="M17 5H9.5a3.5 3.5 0 0 0 0 7h5a3.5 3.5 0 0 1 0 7H6"/></svg></div><div class="feat-t">Unreal Prices</div><div class="feat-d">Netflix $0.70. Crunchyroll Fan $0.20. Nitro promo $0.40. Unmatched pricing.</div></div>
      <div class="feat rv"><div class="feat-ic"><svg width="17" height="17" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="11" width="18" height="11" rx="2" ry="2"/><path d="M7 11V7a5 5 0 0 1 10 0v4"/></svg></div><div class="feat-t">Safe &amp; Discreet</div><div class="feat-d">Delivery through Discord DMs. Clear instructions. Zero unnecessary data collected.</div></div>
      <div class="feat rv"><div class="feat-ic"><svg width="17" height="17" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="22 12 18 12 15 21 9 3 6 12 2 12"/></svg></div><div class="feat-t">Growing Daily</div><div class="feat-d">100+ members and climbing. New products added regularly. Join early.</div></div>
    </div>
  </div>
</section>

<!-- Reviews -->
<section id="reviews">
  <div class="mxc">
    <div class="tc rv">
      <span class="slbl">Customer Feedback</span>
      <h2 class="stit">What Buyers Say</h2>
      <p class="ssub">Real members. Real orders. Real reviews.</p>
    </div>
    <div class="rg">
      <div class="rcard rv"><div class="stars">&#9733;&#9733;&#9733;&#9733;&#9733;</div><p class="rev-t">Nitro promo for $0.40 is insane. Worked instantly. Already told my whole server. Never paying full price again.</p><div class="rev-a"><div class="rev-av">Z</div><div><div class="rev-n">Zakari K.</div><div class="rev-i">NITRO PROMO &middot; VERIFIED</div></div></div></div>
      <div class="rcard rv"><div class="stars">&#9733;&#9733;&#9733;&#9733;&#9733;</div><p class="rev-t">Netflix lifetime for $0.70. Was skeptical but it has been working for weeks. Staff answered my ticket in 2 minutes. Solid shop.</p><div class="rev-a"><div class="rev-av">M</div><div><div class="rev-n">Marcus L.</div><div class="rev-i">NETFLIX LIFETIME &middot; VERIFIED</div></div></div></div>
      <div class="rcard rv"><div class="stars">&#9733;&#9733;&#9733;&#9733;&#9733;</div><p class="rev-t">Got a 2016 Discord account, exactly as described. Good aged, no issues. Will definitely return for more accounts.</p><div class="rev-a"><div class="rev-av">A</div><div><div class="rev-n">Alex S.</div><div class="rev-i">AGED ACCOUNT 2016 &middot; VERIFIED</div></div></div></div>
      <div class="rcard rv"><div class="stars">&#9733;&#9733;&#9733;&#9733;&#9733;</div><p class="rev-t">5000 Robux value for $9 and the account had items worth way more. Already came back for 10k. Shop knows their stock.</p><div class="rev-a"><div class="rev-av">D</div><div><div class="rev-n">Dylan K.</div><div class="rev-i">ROBUX 5K &middot; VERIFIED</div></div></div></div>
      <div class="rcard rv"><div class="stars">&#9733;&#9733;&#9733;&#9733;&#9733;</div><p class="rev-t">Crunchyroll Mega Fan for literally $0.50. Full HD, no ads, working perfectly weeks later. Cannot believe this price is real.</p><div class="rev-a"><div class="rev-av">H</div><div><div class="rev-n">Hina R.</div><div class="rev-i">CRUNCHYROLL MEGA FAN &middot; VERIFIED</div></div></div></div>
      <div class="rcard rv"><div class="stars">&#9733;&#9733;&#9733;&#9733;&#9733;</div><p class="rev-t">Spotify 3 months for $2.50. One of the best shops I have used. Legit products, community that cares, staff respond fast.</p><div class="rev-a"><div class="rev-av">J</div><div><div class="rev-n">Jake T.</div><div class="rev-i">SPOTIFY PREMIUM &middot; VERIFIED</div></div></div></div>
    </div>
  </div>
</section>

<!-- FAQ -->
<section id="faq" style="background:var(--bg2);border-top:1px solid var(--b);border-bottom:1px solid var(--b)">
  <div class="mxc">
    <div class="tc rv">
      <span class="slbl">Questions</span>
      <h2 class="stit">FAQ</h2>
      <p class="ssub">Still stuck? Open a ticket on Discord.</p>
    </div>
    <div class="faq-list rv">
      <div class="fi2"><div class="faq-q">How do I buy something?<div class="faq-ic"><svg width="8" height="8" viewBox="0 0 10 10" fill="none" stroke="currentColor" stroke-width="2.5"><line x1="5" y1="0" x2="5" y2="10"/><line x1="0" y1="5" x2="10" y2="5"/></svg></div></div><div class="faq-a">Click any product card and a slide-up panel will appear with all pricing tiers, step-by-step instructions, and a direct invite to the right Discord channel. Follow the 3 steps, pay, and receive delivery.</div></div>
      <div class="fi2"><div class="faq-q">What payment methods do you accept?<div class="faq-ic"><svg width="8" height="8" viewBox="0 0 10 10" fill="none" stroke="currentColor" stroke-width="2.5"><line x1="5" y1="0" x2="5" y2="10"/><line x1="0" y1="5" x2="10" y2="5"/></svg></div></div><div class="faq-a">Commonly accepted: Crypto (LTC, BTC, USDT) and PayPal F&amp;F. Check the specific product channel for current options. Never send PayPal as Goods and Services.</div></div>
      <div class="fi2"><div class="faq-q">Are refunds available?<div class="faq-ic"><svg width="8" height="8" viewBox="0 0 10 10" fill="none" stroke="currentColor" stroke-width="2.5"><line x1="5" y1="0" x2="5" y2="10"/><line x1="0" y1="5" x2="10" y2="5"/></svg></div></div><div class="faq-a">All sales are final. No refunds after delivery. If a product is dead or invalid on arrival, open a ticket and we will replace it. Chargebacks result in immediate permanent ban.</div></div>
      <div class="fi2"><div class="faq-q">How fast is delivery?<div class="faq-ic"><svg width="8" height="8" viewBox="0 0 10 10" fill="none" stroke="currentColor" stroke-width="2.5"><line x1="5" y1="0" x2="5" y2="10"/><line x1="0" y1="5" x2="10" y2="5"/></svg></div></div><div class="faq-a">Most products land within 5 minutes of payment. Botted members may take slightly longer. If nothing arrives in 20 minutes, open a ticket immediately.</div></div>
      <div class="fi2"><div class="faq-q">What if my product stops working?<div class="faq-ic"><svg width="8" height="8" viewBox="0 0 10 10" fill="none" stroke="currentColor" stroke-width="2.5"><line x1="5" y1="0" x2="5" y2="10"/><line x1="0" y1="5" x2="10" y2="5"/></svg></div></div><div class="faq-a">Third-party platforms can make changes outside our control. If your product stops early through no fault of your own, open a ticket and we will work with you on a replacement where possible.</div></div>
      <div class="fi2"><div class="faq-q">Can I resell products I buy here?<div class="faq-ic"><svg width="8" height="8" viewBox="0 0 10 10" fill="none" stroke="currentColor" stroke-width="2.5"><line x1="5" y1="0" x2="5" y2="10"/><line x1="0" y1="5" x2="10" y2="5"/></svg></div></div><div class="faq-a">Strictly prohibited. Unauthorized reselling, leaking, or redistributing results in immediate permanent blacklisting with no refund. We actively monitor for abuse.</div></div>
    </div>
  </div>
</section>

<!-- Discord CTA -->
<section id="dcta">
  <div class="mxc">
    <div class="dbox rv">
      <span class="slbl">Ready?</span>
      <h2 class="stit" style="margin-bottom:8px">Join Retro Hub</h2>
      <p style="font-size:12.5px;color:var(--t2);font-family:var(--fm)">100+ members &middot; 9 product categories &middot; Fast support &middot; Growing daily</p>
      <div class="dinv">
        <span class="dinv-l">discord.gg/DfU3ZQNgAV</span>
        <button class="dinv-c" id="dcbtn">COPY</button>
      </div>
      <a href="https://discord.gg/DfU3ZQNgAV" target="_blank" rel="noopener" class="btn-p" style="display:inline-flex">
        <svg width="15" height="15" viewBox="0 0 24 24" fill="currentColor"><path d="M20.317 4.37a19.791 19.791 0 0 0-4.885-1.515.074.074 0 0 0-.079.037c-.21.375-.444.864-.608 1.25a18.27 18.27 0 0 0-5.487 0 12.64 12.64 0 0 0-.617-1.25.077.077 0 0 0-.079-.037A19.736 19.736 0 0 0 3.677 4.37a.07.07 0 0 0-.032.027C.533 9.046-.32 13.58.099 18.057.1 18.08.114 18.1.135 18.115a19.9 19.9 0 0 0 5.993 3.03.078.078 0 0 0 .084-.028c.462-.63.874-1.295 1.226-1.994a.076.076 0 0 0-.041-.106 13.107 13.107 0 0 1-1.872-.892.077.077 0 0 1-.008-.128 10.2 10.2 0 0 0 .372-.292.074.074 0 0 1 .077-.01c3.928 1.793 8.18 1.793 12.062 0a.074.074 0 0 1 .078.01c.12.098.246.198.373.292a.077.077 0 0 1-.006.127 12.299 12.299 0 0 1-1.873.892.077.077 0 0 0-.041.107c.36.698.772 1.362 1.225 1.993a.076.076 0 0 0 .084.028 19.839 19.839 0 0 0 6.002-3.03.077.077 0 0 0 .032-.054c.5-5.177-.838-9.674-3.549-13.66a.061.061 0 0 0-.031-.03z"/></svg>
        JOIN RETRO HUB
      </a>
      <p style="font-family:var(--fm);font-size:9.5px;color:var(--t3);margin-top:14px">Free to join &middot; Real support &middot; Lowest prices guaranteed</p>
    </div>
  </div>
</section>

<!-- Footer -->
<footer>
  <div class="fg2">
    <div class="fb">
      <a href="#" class="brand">
        <svg style="width:26px;height:26px;filter:drop-shadow(0 0 5px #c8001a)" viewBox="0 0 100 100" fill="none">
          <path d="M22 75V25H52C62 25 70 33 70 43C70 50 66 56 60 59L72 75H58L47 61H36V75H22ZM36 49H50C54 49 57 46 57 42C57 38 54 35 50 35H36V49Z" fill="#c8001a"/>
          <path d="M60 59L72 75H58" fill="#7a000f"/>
        </svg>
        <span class="brand-name" style="font-size:17px">RETRO <b>HUB</b></span>
      </a>
      <p>Premium digital services at prices nobody else offers. Trusted Discord shop with fast delivery.</p>
    </div>
    <div class="fc2"><h4>Products</h4><ul>
      <li><a href="https://discord.gg/MZb4QfC5Au" target="_blank" rel="noopener">Discord Nitro</a></li>
      <li><a href="https://discord.gg/a7nGt94Gr" target="_blank" rel="noopener">Discord Decos</a></li>
      <li><a href="https://discord.gg/7qSrg3u2YD" target="_blank" rel="noopener">Aged Accounts</a></li>
      <li><a href="https://discord.gg/cCWtt25Tm7" target="_blank" rel="noopener">Botted Members</a></li>
      <li><a href="https://discord.gg/fj3H6DpWZt" target="_blank" rel="noopener">Crypto Flasher</a></li>
      <li><a href="https://discord.gg/X2RSAeKz2k" target="_blank" rel="noopener">Crunchyroll</a></li>
      <li><a href="https://discord.gg/6HDV39gmaV" target="_blank" rel="noopener">Netflix</a></li>
      <li><a href="https://discord.gg/TbWBUwF3G6" target="_blank" rel="noopener">Followers</a></li>
      <li><a href="https://discord.gg/kxGUTDR449" target="_blank" rel="noopener">Robux</a></li>
    </ul></div>
    <div class="fc2"><h4>Support</h4><ul>
      <li><a href="https://discord.gg/DfU3ZQNgAV" target="_blank" rel="noopener">Open a Ticket</a></li>
      <li><a href="https://discord.gg/DfU3ZQNgAV" target="_blank" rel="noopener">Order Status</a></li>
      <li><a href="https://discord.gg/DfU3ZQNgAV" target="_blank" rel="noopener">Replacements</a></li>
      <li><a href="https://discord.gg/DfU3ZQNgAV" target="_blank" rel="noopener">Contact Staff</a></li>
    </ul></div>
    <div class="fc2"><h4>Legal</h4><ul>
      <li><a href="#" id="tos-rop">Terms of Service</a></li>
      <li><a href="#">Privacy Policy</a></li>
      <li><a href="#">Refund Policy</a></li>
    </ul></div>
  </div>
  <div class="fbot">
    <p>&copy; 2025 Retro Hub. All rights reserved.</p>
    <div class="obadge"><div class="gdot"></div>ALL SYSTEMS ONLINE</div>
  </div>
  <p class="disc-n">Retro Hub is an independent digital goods reseller not affiliated with Discord, Spotify, Netflix, Roblox, Crunchyroll, Instagram, TikTok, or Twitch. All trademarks are property of their respective owners. All sales are final. By purchasing you agree to our Terms of Service.</p>
</footer>

<a href="https://discord.gg/DfU3ZQNgAV" target="_blank" rel="noopener" id="fdisc" title="Join Discord">
  <svg width="19" height="19" viewBox="0 0 24 24" fill="white">
    <path d="M20.317 4.37a19.791 19.791 0 0 0-4.885-1.515.074.074 0 0 0-.079.037c-.21.375-.444.864-.608 1.25a18.27 18.27 0 0 0-5.487 0 12.64 12.64 0 0 0-.617-1.25.077.077 0 0 0-.079-.037A19.736 19.736 0 0 0 3.677 4.37a.07.07 0 0 0-.032.027C.533 9.046-.32 13.58.099 18.057.1 18.08.114 18.1.135 18.115a19.9 19.9 0 0 0 5.993 3.03.078.078 0 0 0 .084-.028c.462-.63.874-1.295 1.226-1.994a.076.076 0 0 0-.041-.106 13.107 13.107 0 0 1-1.872-.892.077.077 0 0 1-.008-.128 10.2 10.2 0 0 0 .372-.292.074.074 0 0 1 .077-.01c3.928 1.793 8.18 1.793 12.062 0a.074.074 0 0 1 .078.01c.12.098.246.198.373.292a.077.077 0 0 1-.006.127 12.299 12.299 0 0 1-1.873.892.077.077 0 0 0-.041.107c.36.698.772 1.362 1.225 1.993a.076.076 0 0 0 .084.028 19.839 19.839 0 0 0 6.002-3.03.077.077 0 0 0 .032-.054c.5-5.177-.838-9.674-3.549-13.66a.061.061 0 0 0-.031-.03z"/>
  </svg>
</a>

<script>
/* ================================================================
   STEP 1 — DATA
   ================================================================ */
var PRODUCTS = [
  {id:"nitro",    cat:"discord",   ico:"purple_heart", name:"Discord Nitro",       sub:"All tiers - Instant delivery",           badge:"hot",  url:"https://discord.gg/MZb4QfC5Au", inv:"discord.gg/MZb4QfC5Au",
   prices:[{l:"Nitro Boost",p:"$3.80"},{l:"Nitro Basic",p:"$1.30"},{l:"Promo 1 Month",p:"$0.40"},{l:"Promo 3 Months",p:"$1.30"}]},
  {id:"decos",    cat:"discord",   ico:"sparkles",     name:"Discord Decorations", sub:"Profile decos - Big discounts vs retail", badge:"new",  url:"https://discord.gg/a7nGt94Gr", inv:"discord.gg/a7nGt94Gr",
   prices:[{l:"Retail $4.99",p:"$1.70"},{l:"Retail $5.99",p:"$2.00"},{l:"Retail $6.99",p:"$2.60"},{l:"Retail $7.99",p:"$2.90"},{l:"Retail $8.49",p:"$3.20"},{l:"Retail $9.99",p:"$3.70"},{l:"Retail $11.99",p:"$4.00"}]},
  {id:"aged",     cat:"discord",   ico:"bank",         name:"Aged Discord Accounts",sub:"Vintage accounts - Higher trust value",  badge:null,   url:"https://discord.gg/7qSrg3u2YD", inv:"discord.gg/7qSrg3u2YD",
   prices:[{l:"2020 Account",p:"$1.00"},{l:"2019 Account",p:"$2.00"},{l:"2018 Account",p:"$3.00"},{l:"2017 Account",p:"$4.50"},{l:"2016 Account",p:"$11.00"}]},
  {id:"botted",   cat:"discord",   ico:"group",        name:"Botted Members",      sub:"Boost server count - Open ticket to order",badge:"bulk", url:"https://discord.gg/cCWtt25Tm7", inv:"discord.gg/cCWtt25Tm7",
   prices:[{l:"1,000 Offline",p:"$1.00"},{l:"1,000 Online",p:"$2.00"}]},
  {id:"crypto",   cat:"crypto",    ico:"coin",         name:"Crypto Flasher",      sub:"Flash credits - Bulk discounts",          badge:"hot",  url:"https://discord.gg/fj3H6DpWZt", inv:"discord.gg/fj3H6DpWZt",
   prices:[{l:"1 Use",p:"$0.20"},{l:"10 Uses",p:"$1.00"},{l:"50 Uses",p:"$3.50"},{l:"100 Uses",p:"$7.00"},{l:"200 Uses",p:"$13.00"},{l:"Unlimited",p:"$35.00"}]},
  {id:"crunchy",  cat:"streaming", ico:"anime",        name:"Crunchyroll",         sub:"Ad-free anime - Fan and Mega Fan plans",  badge:null,   url:"https://discord.gg/X2RSAeKz2k", inv:"discord.gg/X2RSAeKz2k",
   prices:[{l:"Fan Plan",p:"$0.20"},{l:"Mega Fan Plan",p:"$0.50"}]},
  {id:"netflix",  cat:"streaming", ico:"film",         name:"Netflix",             sub:"Lifetime access - One-time payment",     badge:"hot",  url:"https://discord.gg/6HDV39gmaV", inv:"discord.gg/6HDV39gmaV",
   prices:[{l:"Netflix Lifetime",p:"$0.70"}]},
  {id:"follows",  cat:"social",    ico:"chart",        name:"Followers and Likes", sub:"Instagram, TikTok and Twitch accounts",  badge:"new",  url:"https://discord.gg/TbWBUwF3G6", inv:"discord.gg/TbWBUwF3G6",
   prices:[{l:"1K Instagram",p:"$6.00"},{l:"1K TikTok",p:"$4.50"},{l:"Twitch 2K",p:"$2.00"},{l:"Twitch 5K",p:"$2.50"},{l:"Twitch 9K",p:"$3.00"}]},
  {id:"robux",    cat:"gaming",    ico:"game",         name:"Robux",               sub:"Roblox item accounts - 32K in stock",    badge:"hot",  url:"https://discord.gg/kxGUTDR449", inv:"discord.gg/kxGUTDR449",
   prices:[{l:"1,000 Robux value",p:"$3.50"},{l:"2,500 Robux value",p:"$6.00"},{l:"5,000 Robux value",p:"$9.00"},{l:"10,000 Robux value",p:"$13.50"},{l:"50,000+ Robux value",p:"$35.00"}]},
  {id:"spotify",  cat:"streaming", ico:"music",        name:"Spotify Premium",     sub:"3 months ad-free - Best value deal",    badge:null,   url:"https://discord.gg/DfU3ZQNgAV", inv:"discord.gg/DfU3ZQNgAV",
   prices:[{l:"3 Months Premium",p:"$2.50"}]}
];

var EMOJIS = {
  purple_heart:"💜", sparkles:"✨", bank:"🏛️", group:"👥",
  coin:"₿", anime:"🍥", film:"🎬", chart:"📈", game:"🎮", music:"🎵"
};

/* ================================================================
   STEP 2 — OBSERVERS (must be created BEFORE renderCards is called)
   ================================================================ */
var ro = new IntersectionObserver(function(entries) {
  entries.forEach(function(e) {
    if (e.isIntersecting) { e.target.classList.add("vis"); ro.unobserve(e.target); }
  });
}, {threshold: 0.07, rootMargin: "0px 0px -28px 0px"});

/* Observe all existing .rv elements */
document.querySelectorAll(".rv").forEach(function(el) { ro.observe(el); });

var co = new IntersectionObserver(function(entries) {
  entries.forEach(function(e) {
    if (e.isIntersecting) {
      var el = e.target;
      var target = parseInt(el.getAttribute("data-t"), 10);
      var val = 0;
      var step = target / 80;
      var ti = setInterval(function() {
        val += step;
        if (val >= target) { val = target; clearInterval(ti); }
        el.textContent = Math.floor(val).toLocaleString();
      }, 16);
      co.unobserve(el);
    }
  });
}, {threshold: 0.6});
document.querySelectorAll(".ctr").forEach(function(c) { co.observe(c); });

/* ================================================================
   STEP 3 — RENDER CARDS
   ================================================================ */
var currentProd = null;

function makeDscSVG() {
  var ns = "http://www.w3.org/2000/svg";
  var svg = document.createElementNS(ns, "svg");
  svg.setAttribute("width", "13");
  svg.setAttribute("height", "13");
  svg.setAttribute("viewBox", "0 0 24 24");
  svg.setAttribute("fill", "currentColor");
  var p = document.createElementNS(ns, "path");
  p.setAttribute("d", "M20.317 4.37a19.791 19.791 0 0 0-4.885-1.515.074.074 0 0 0-.079.037c-.21.375-.444.864-.608 1.25a18.27 18.27 0 0 0-5.487 0 12.64 12.64 0 0 0-.617-1.25.077.077 0 0 0-.079-.037A19.736 19.736 0 0 0 3.677 4.37a.07.07 0 0 0-.032.027C.533 9.046-.32 13.58.099 18.057.1 18.08.114 18.1.135 18.115a19.9 19.9 0 0 0 5.993 3.03.078.078 0 0 0 .084-.028c.462-.63.874-1.295 1.226-1.994a.076.076 0 0 0-.041-.106 13.107 13.107 0 0 1-1.872-.892.077.077 0 0 1-.008-.128 10.2 10.2 0 0 0 .372-.292.074.074 0 0 1 .077-.01c3.928 1.793 8.18 1.793 12.062 0a.074.074 0 0 1 .078.01c.12.098.246.198.373.292a.077.077 0 0 1-.006.127 12.299 12.299 0 0 1-1.873.892.077.077 0 0 0-.041.107c.36.698.772 1.362 1.225 1.993a.076.076 0 0 0 .084.028 19.839 19.839 0 0 0 6.002-3.03.077.077 0 0 0 .032-.054c.5-5.177-.838-9.674-3.549-13.66a.061.061 0 0 0-.031-.03z");
  svg.appendChild(p);
  return svg;
}

function renderCards(data) {
  var grid = document.getElementById("pgrid");
  grid.innerHTML = "";

  if (!data.length) {
    var empty = document.createElement("p");
    empty.style.cssText = "color:var(--t3);font-family:var(--fm);font-size:13px;padding:24px 0";
    empty.textContent = "No products match your search.";
    grid.appendChild(empty);
    return;
  }

  data.forEach(function(p) {
    var card = document.createElement("div");
    card.className = "pcard rv";
    card.setAttribute("data-cat", p.cat);

    /* --- top --- */
    var top = document.createElement("div");
    top.className = "pc-top";
    var ico = document.createElement("div");
    ico.className = "pc-ico";
    ico.textContent = EMOJIS[p.ico] || "📦";
    top.appendChild(ico);
    if (p.badge) {
      var bdg = document.createElement("span");
      var bmap = {hot:"bh", new:"bn", bulk:"bb"};
      var blbl = {hot:"HOT", new:"NEW", bulk:"BULK"};
      bdg.className = "pbadge " + (bmap[p.badge] || "bh");
      bdg.textContent = blbl[p.badge] || p.badge.toUpperCase();
      top.appendChild(bdg);
    }
    card.appendChild(top);

    /* --- body --- */
    var body = document.createElement("div");
    body.className = "pc-body";
    var nm = document.createElement("div");
    nm.className = "pc-name";
    nm.textContent = p.name;
    body.appendChild(nm);
    var sb = document.createElement("div");
    sb.className = "pc-sub";
    sb.textContent = p.sub;
    body.appendChild(sb);

    if (p.prices.length === 1) {
      var big = document.createElement("div");
      big.className = "pc-price-big";
      big.textContent = p.prices[0].p;
      body.appendChild(big);
      var was = document.createElement("div");
      was.className = "pc-price-was";
      was.textContent = p.prices[0].l;
      body.appendChild(was);
    } else {
      var rows = document.createElement("div");
      rows.className = "prows";
      var showCount = Math.min(p.prices.length, 4);
      for (var i = 0; i < showCount; i++) {
        var r = p.prices[i];
        var row = document.createElement("div");
        row.className = "prow";
        var rl = document.createElement("span");
        rl.className = "prow-l";
        rl.textContent = r.l;
        var rp = document.createElement("span");
        rp.className = "prow-p";
        rp.textContent = r.p;
        row.appendChild(rl);
        row.appendChild(rp);
        rows.appendChild(row);
      }
      if (p.prices.length > 4) {
        var more = document.createElement("div");
        more.className = "prow";
        more.style.cssText = "justify-content:center;color:var(--t3);font-family:var(--fm);font-size:9.5px";
        more.textContent = "+" + (p.prices.length - 4) + " more tiers inside";
        rows.appendChild(more);
      }
      body.appendChild(rows);
    }
    card.appendChild(body);

    /* --- foot --- */
    var foot = document.createElement("div");
    foot.className = "pc-foot";
    var btn = document.createElement("button");
    btn.className = "pc-buybtn";
    btn.setAttribute("data-id", p.id);
    var inner = document.createElement("span");
    inner.className = "bi";
    inner.appendChild(makeDscSVG());
    inner.appendChild(document.createTextNode(" BUY IN CHANNEL"));
    btn.appendChild(inner);
    foot.appendChild(btn);
    card.appendChild(foot);
    grid.appendChild(card);
  });

  /* observe new cards */
  document.querySelectorAll(".pcard.rv").forEach(function(el) { ro.observe(el); });
  attachTilt();

  /* buy button listeners */
  document.querySelectorAll(".pc-buybtn").forEach(function(btn) {
    btn.addEventListener("click", function(e) {
      e.stopPropagation();
      openModal(this.getAttribute("data-id"));
    });
  });
}

/* Initial render */
renderCards(PRODUCTS);

/* ================================================================
   STEP 4 — CHANNEL MODAL
   ================================================================ */
function openModal(id) {
  var p = null;
  for (var i = 0; i < PRODUCTS.length; i++) {
    if (PRODUCTS[i].id === id) { p = PRODUCTS[i]; break; }
  }
  if (!p) return;
  currentProd = p;

  document.getElementById("chan-ico").textContent  = EMOJIS[p.ico] || "📦";
  document.getElementById("chan-name").textContent  = p.name;
  document.getElementById("chan-subt").textContent  = "RETRO HUB - " + p.sub.toUpperCase();
  document.getElementById("chan-url").textContent   = p.inv;
  document.getElementById("chan-go").href           = p.url;

  var pills = document.getElementById("chan-pills");
  pills.innerHTML = "";
  p.prices.forEach(function(pr, i) {
    var pill = document.createElement("div");
    pill.className = "cpill" + (i === 0 ? " sel" : "");
    var lbl = document.createElement("span");
    lbl.className = "cpill-l";
    lbl.textContent = pr.l;
    var prc = document.createElement("div");
    prc.className = "cpill-p";
    prc.textContent = pr.p;
    var chk = document.createElement("div");
    chk.className = "cpill-chk";
    chk.textContent = "\u2713";
    pill.appendChild(lbl);
    pill.appendChild(prc);
    pill.appendChild(chk);
    pill.addEventListener("click", function() {
      pills.querySelectorAll(".cpill").forEach(function(x) { x.classList.remove("sel"); });
      pill.classList.add("sel");
    });
    pills.appendChild(pill);
  });

  var cpy = document.getElementById("chan-cpy");
  cpy.textContent = "COPY";
  cpy.classList.remove("ok");

  document.getElementById("chan").classList.remove("off");
  document.body.style.overflow = "hidden";
}

function closeModal() {
  document.getElementById("chan").classList.add("off");
  document.body.style.overflow = "";
}

document.getElementById("chan-cls").addEventListener("click", closeModal);
document.getElementById("chan-bg").addEventListener("click",  closeModal);

document.getElementById("chan-cpy").addEventListener("click", function() {
  if (!currentProd) return;
  try { navigator.clipboard.writeText("https://" + currentProd.inv); } catch(e) {}
  this.textContent = "COPIED!";
  this.classList.add("ok");
  var self = this;
  setTimeout(function() { self.textContent = "COPY"; self.classList.remove("ok"); }, 2400);
});

/* swipe down to close */
var touchStartY = 0;
document.querySelector(".chan-box").addEventListener("touchstart", function(e) {
  touchStartY = e.touches[0].clientY;
}, {passive: true});
document.querySelector(".chan-box").addEventListener("touchend", function(e) {
  if (e.changedTouches[0].clientY - touchStartY > 70) closeModal();
}, {passive: true});

/* ================================================================
   STEP 5 — LOADING BAR
   ================================================================ */
var ldb  = document.getElementById("ldb");
var ldel = document.getElementById("ld");
var lp = 0;
var ldi = setInterval(function() {
  lp += Math.random() * 13 + 5;
  if (lp >= 100) {
    lp = 100;
    clearInterval(ldi);
    setTimeout(function() { ldel.classList.add("off"); }, 300);
  }
  ldb.style.width = lp + "%";
}, 90);

/* ================================================================
   STEP 6 — TOS
   ================================================================ */
(function() {
  var ov = document.getElementById("tos");
  if (localStorage.getItem("rh_tos")) { ov.classList.add("off"); return; }
  document.body.style.overflow = "hidden";
  var checked = false;
  document.getElementById("tcrow").addEventListener("click", function() {
    checked = !checked;
    this.classList.toggle("on", checked);
    document.getElementById("ta").disabled = !checked;
  });
  document.getElementById("ta").addEventListener("click", function() {
    if (!checked) return;
    localStorage.setItem("rh_tos", "1");
    localStorage.setItem("rh_tos_ts", new Date().toISOString());
    ov.classList.add("off");
    document.body.style.overflow = "";
  });
})();

document.getElementById("tos-rop").addEventListener("click", function(e) {
  e.preventDefault();
  document.getElementById("tos").classList.remove("off");
});

/* ================================================================
   STEP 7 — NAVBAR
   ================================================================ */
var navEl  = document.getElementById("nav");
var hamEl  = document.getElementById("ham");
var mmEl   = document.getElementById("mmnav");
window.addEventListener("scroll", function() {
  navEl.classList.toggle("scr", window.scrollY > 20);
}, {passive: true});
hamEl.addEventListener("click", function() {
  this.classList.toggle("open");
  mmEl.classList.toggle("open");
});
mmEl.querySelectorAll("a").forEach(function(a) {
  a.addEventListener("click", function() {
    hamEl.classList.remove("open");
    mmEl.classList.remove("open");
  });
});
window.addEventListener("scroll", function() {
  if (mmEl.classList.contains("open")) {
    hamEl.classList.remove("open");
    mmEl.classList.remove("open");
  }
}, {passive: true});

/* ================================================================
   STEP 8 — CURSOR
   ================================================================ */
var curDot  = document.getElementById("cur");
var curRing = document.getElementById("cur2");
var mx = 0, my = 0, cx = 0, cy = 0;
window.addEventListener("mousemove", function(e) {
  mx = e.clientX; my = e.clientY;
  curDot.style.left = mx + "px";
  curDot.style.top  = my + "px";
}, {passive: true});
(function animCursor() {
  cx += (mx - cx) * 0.12;
  cy += (my - cy) * 0.12;
  curRing.style.left = cx + "px";
  curRing.style.top  = cy + "px";
  requestAnimationFrame(animCursor);
})();

/* ================================================================
   STEP 9 — TILT
   ================================================================ */
function attachTilt() {
  document.querySelectorAll(".pcard, .feat, .rcard").forEach(function(card) {
    card.onmousemove = function(e) {
      var r = card.getBoundingClientRect();
      var x = (e.clientX - r.left) / r.width  - 0.5;
      var y = (e.clientY - r.top)  / r.height - 0.5;
      card.style.transform = "perspective(480px) rotateY(" + (x * 6) + "deg) rotateX(" + (-y * 6) + "deg) translateY(-5px)";
    };
    card.onmouseleave = function() { card.style.transform = ""; };
  });
}
attachTilt();

/* ================================================================
   STEP 10 — SEARCH + FILTER
   ================================================================ */
var currentCat = "all";
var siEl = document.getElementById("si");
document.getElementById("ctabs").addEventListener("click", function(e) {
  if (!e.target.matches(".ctab")) return;
  document.querySelectorAll(".ctab").forEach(function(b) { b.classList.remove("on"); });
  e.target.classList.add("on");
  currentCat = e.target.getAttribute("data-cat");
  doFilter();
});
siEl.addEventListener("input", doFilter);
function doFilter() {
  var q = siEl.value.toLowerCase();
  var filtered = PRODUCTS.filter(function(p) {
    var catMatch  = (currentCat === "all" || p.cat === currentCat);
    var txtMatch  = (!q || p.name.toLowerCase().indexOf(q) !== -1 || p.sub.toLowerCase().indexOf(q) !== -1);
    return catMatch && txtMatch;
  });
  renderCards(filtered);
}

/* ================================================================
   STEP 11 — FAQ
   ================================================================ */
document.querySelectorAll(".faq-q").forEach(function(q) {
  q.addEventListener("click", function() {
    var it   = q.parentElement;
    var open = it.classList.contains("open");
    document.querySelectorAll(".fi2.open").forEach(function(x) { x.classList.remove("open"); });
    if (!open) it.classList.add("open");
  });
});

/* ================================================================
   STEP 12 — COPY CTA BUTTON
   ================================================================ */
document.getElementById("dcbtn").addEventListener("click", function() {
  try { navigator.clipboard.writeText("https://discord.gg/DfU3ZQNgAV"); } catch(e) {}
  this.textContent = "COPIED!";
  this.classList.add("ok");
  var self = this;
  setTimeout(function() { self.textContent = "COPY"; self.classList.remove("ok"); }, 2400);
});

/* ================================================================
   STEP 13 — SOUND TOGGLE
   ================================================================ */
var soundOn = false;
document.getElementById("sb").addEventListener("click", function() {
  soundOn = !soundOn;
  document.getElementById("son").style.display  = soundOn ? "block" : "none";
  document.getElementById("soff").style.display = soundOn ? "none"  : "block";
});

/* ================================================================
   STEP 14 — LIVE NOTIFICATIONS
   ================================================================ */
(function() {
  var buys = [
    {u:"Z***k", p:"Nitro Promo 1 Month",   t:"just now"},
    {u:"M***s", p:"Netflix Lifetime",      t:"1m ago"},
    {u:"A***x", p:"2018 Discord Account",  t:"just now"},
    {u:"D***n", p:"5000 Robux",            t:"2m ago"},
    {u:"H***a", p:"Crunchyroll Mega Fan",  t:"just now"},
    {u:"J***e", p:"Spotify 3 Months",      t:"3m ago"},
    {u:"R***l", p:"Nitro Basic",           t:"just now"},
    {u:"S***h", p:"1K TikTok Followers",   t:"1m ago"},
    {u:"T***o", p:"100 Crypto Uses",       t:"just now"},
    {u:"K***i", p:"Discord Decorations",   t:"2m ago"},
    {u:"B***y", p:"1000 Online Members",   t:"just now"},
    {u:"P***s", p:"10000 Robux",           t:"4m ago"},
    {u:"L***a", p:"Twitch 5K Account",     t:"just now"},
    {u:"F***r", p:"2016 Discord Account",  t:"1m ago"}
  ];
  var nc = document.getElementById("nc");
  function showNotif() {
    var b = buys[Math.floor(Math.random() * buys.length)];
    var card = document.createElement("div");
    card.className = "ncard";
    var av  = document.createElement("div"); av.className  = "nav2"; av.textContent = b.u[0];
    var ct  = document.createElement("div"); ct.className  = "nct";
    var p1  = document.createElement("p");   p1.textContent = b.u + " purchased";
    var sp  = document.createElement("span"); sp.textContent = b.p;
    var sm  = document.createElement("small"); sm.textContent = b.t;
    ct.appendChild(p1); ct.appendChild(sp); ct.appendChild(sm);
    card.appendChild(av); card.appendChild(ct);
    nc.appendChild(card);
    setTimeout(function() {
      card.classList.add("out");
      setTimeout(function() { if (card.parentNode) card.parentNode.removeChild(card); }, 300);
    }, 4000);
  }
  setTimeout(function() {
    showNotif();
    setInterval(showNotif, 7000 + Math.random() * 4000);
  }, 3000);
})();

/* ================================================================
   STEP 15 — PARTICLES
   ================================================================ */
(function() {
  var canvas = document.createElement("canvas");
  canvas.style.cssText = "position:fixed;inset:0;pointer-events:none;z-index:0;opacity:.28";
  document.body.appendChild(canvas);
  var ctx = canvas.getContext("2d");
  var W, H, particles = [];
  function resize() { W = canvas.width = window.innerWidth; H = canvas.height = window.innerHeight; }
  resize();
  window.addEventListener("resize", resize, {passive: true});
  function Particle() { this.reset(); }
  Particle.prototype.reset = function() {
    this.x   = Math.random() * W;
    this.y   = Math.random() * H;
    this.s   = Math.random() * 1.1 + 0.2;
    this.vx  = (Math.random() - 0.5) * 0.22;
    this.vy  = (Math.random() - 0.5) * 0.22;
    this.o   = Math.random() * 0.35 + 0.07;
    this.col = Math.random() < 0.24 ? "#c8001a" : "#ffffff";
  };
  Particle.prototype.update = function() {
    this.x += this.vx; this.y += this.vy;
    if (this.x < 0 || this.x > W || this.y < 0 || this.y > H) this.reset();
  };
  Particle.prototype.draw = function() {
    ctx.beginPath();
    ctx.arc(this.x, this.y, this.s, 0, Math.PI * 2);
    ctx.fillStyle = this.col;
    ctx.globalAlpha = this.o;
    ctx.fill();
  };
  for (var i = 0; i < 85; i++) { particles.push(new Particle()); }
  function animParticles() {
    ctx.clearRect(0, 0, W, H);
    ctx.globalAlpha = 1;
    particles.forEach(function(p) { p.update(); p.draw(); });
    requestAnimationFrame(animParticles);
  }
  animParticles();
})();
</script>
</body>
</html>

<!DOCTYPE html>
<html lang="vi">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>PMAX Agency – Brief Request</title>
<link href="https://fonts.googleapis.com/css2?family=Be+Vietnam+Pro:wght@300;400;500;600;700;800&family=DM+Mono:wght@400;500&display=swap" rel="stylesheet">
<style>
  :root {
    --pmax-blue:        #0033A0;
    --pmax-blue-light:  #1A4FBF;
    --pmax-blue-pale:   #EBF0FA;
    --pmax-orange:      #FF6B00;
    --pmax-orange-pale: #FFF3E8;
    --pmax-dark:        #0A1628;
    --pmax-gray-700:    #3D4E6B;
    --pmax-gray-500:    #7A8BAA;
    --pmax-gray-200:    #E0E6F0;
    --pmax-gray-100:    #F4F6FB;
    --pmax-white:       #FFFFFF;
    --radius: 12px;
    --radius-sm: 8px;
    --shadow-card: 0 2px 20px rgba(0,51,160,0.07);
    --transition: all 0.22s cubic-bezier(0.4,0,0.2,1);
  }
  *,*::before,*::after{box-sizing:border-box;margin:0;padding:0}
  body{font-family:'Be Vietnam Pro',sans-serif;background:var(--pmax-gray-100);color:var(--pmax-dark);min-height:100vh;-webkit-font-smoothing:antialiased}
  .site-header{background:var(--pmax-white);border-bottom:3px solid var(--pmax-blue);padding:0 24px;position:sticky;top:0;z-index:100}
  .header-inner{max-width:780px;margin:0 auto;height:72px;display:flex;align-items:center;justify-content:space-between}
  .logo{display:flex;align-items:center;gap:10px;text-decoration:none}
  .logo-img{height:56px;width:auto;display:block}
  .header-tag{font-size:12px;font-weight:500;color:var(--pmax-blue);background:var(--pmax-blue-pale);padding:4px 12px;border-radius:99px;border:1px solid rgba(0,51,160,0.15)}
  .hero{background:linear-gradient(135deg,#0033A0 0%,#0047CC 65%,#1A6FD4 100%);border-bottom:4px solid var(--pmax-orange);padding:40px 24px 32px}
  .hero-inner{max-width:780px;margin:0 auto}
  .hero-eyebrow{display:inline-flex;align-items:center;gap:6px;font-size:12px;font-weight:600;color:rgba(255,255,255,0.85);text-transform:uppercase;letter-spacing:1.2px;margin-bottom:12px}
  .hero-eyebrow::before{content:'';width:18px;height:2px;background:var(--pmax-orange);border-radius:2px}
  .hero h1{font-size:clamp(22px,4vw,32px);font-weight:800;color:#fff;line-height:1.2;letter-spacing:-0.8px;margin-bottom:8px}
  .hero p{font-size:14px;color:rgba(255,255,255,0.75);line-height:1.6;max-width:480px}
  .progress-wrap{max-width:780px;margin:0 auto;padding:24px 24px 0}
  .progress-info{display:flex;justify-content:space-between;align-items:center;margin-bottom:8px}
  .progress-label{font-size:12px;font-weight:600;color:var(--pmax-gray-500);letter-spacing:0.3px}
  .progress-count{font-size:12px;font-weight:600;color:var(--pmax-blue);font-family:'DM Mono',monospace}
  .progress-bar{height:5px;background:var(--pmax-gray-200);border-radius:99px;overflow:hidden}
  .progress-fill{height:100%;background:linear-gradient(90deg,var(--pmax-blue),var(--pmax-orange));border-radius:99px;transition:width 0.5s cubic-bezier(0.4,0,0.2,1);width:0%}
  .stepper{max-width:780px;margin:0 auto;padding:16px 24px 0;display:flex;gap:6px;overflow-x:auto;scrollbar-width:none;-ms-overflow-style:none}
  .stepper::-webkit-scrollbar{display:none}
  .step-btn{flex:none;display:flex;align-items:center;gap:7px;padding:7px 12px;border-radius:99px;border:1.5px solid transparent;background:transparent;font-family:'Be Vietnam Pro',sans-serif;font-size:12px;font-weight:500;color:var(--pmax-gray-500);cursor:pointer;transition:var(--transition);white-space:nowrap}
  .step-btn .step-num{width:20px;height:20px;border-radius:50%;background:var(--pmax-gray-200);display:flex;align-items:center;justify-content:center;font-size:11px;font-weight:700;font-family:'DM Mono',monospace;color:var(--pmax-gray-500);transition:var(--transition);flex-shrink:0}
  .step-btn.active{border-color:var(--pmax-blue);background:var(--pmax-blue-pale);color:var(--pmax-blue)}
  .step-btn.active .step-num{background:var(--pmax-blue);color:white}
  .step-btn.done{color:var(--pmax-gray-700);border-color:var(--pmax-gray-200);background:var(--pmax-white)}
  .step-btn.done .step-num{background:#22C55E;color:white}
  .main{max-width:780px;margin:0 auto;padding:20px 24px}
  .section-card{background:var(--pmax-white);border-radius:var(--radius);border:1px solid var(--pmax-gray-200);box-shadow:var(--shadow-card);overflow:hidden;margin-bottom:16px;display:none;animation:fadeUp 0.28s ease}
  .section-card.active{display:block}
  @keyframes fadeUp{from{opacity:0;transform:translateY(10px)}to{opacity:1;transform:translateY(0)}}
  .section-header{padding:22px 28px 18px;border-bottom:1px solid var(--pmax-gray-100);display:flex;align-items:flex-start;gap:14px}
  .section-icon{width:42px;height:42px;background:var(--pmax-blue-pale);border-radius:10px;display:flex;align-items:center;justify-content:center;font-size:19px;flex-shrink:0}
  .section-label{font-size:11px;font-weight:700;color:var(--pmax-blue);text-transform:uppercase;letter-spacing:1px;margin-bottom:3px}
  .section-title{font-size:17px;font-weight:700;color:var(--pmax-dark);letter-spacing:-0.3px}
  .section-desc{font-size:13px;color:var(--pmax-gray-500);margin-top:3px;line-height:1.5}
  .section-body{padding:22px 28px;display:flex;flex-direction:column;gap:18px}
  .field{display:flex;flex-direction:column;gap:6px}
  .field-row{display:grid;grid-template-columns:1fr 1fr;gap:14px}
  @media(max-width:560px){.field-row{grid-template-columns:1fr}}
  label{font-size:13.5px;font-weight:600;color:var(--pmax-dark);display:flex;align-items:center;gap:5px}
  label .req{color:var(--pmax-orange);font-size:14px;line-height:1}
  .hint{font-size:12px;color:var(--pmax-gray-500);line-height:1.5;margin-top:-2px}
  input[type="text"],input[type="email"],input[type="tel"],input[type="date"],select,textarea{font-family:'Be Vietnam Pro',sans-serif;font-size:14px;color:var(--pmax-dark);background:var(--pmax-gray-100);border:1.5px solid transparent;border-radius:var(--radius-sm);padding:11px 14px;width:100%;transition:var(--transition);outline:none;-webkit-appearance:none}
  input:focus,select:focus,textarea:focus{background:var(--pmax-white);border-color:var(--pmax-blue);box-shadow:0 0 0 3px rgba(0,51,160,0.10)}
  input::placeholder,textarea::placeholder{color:var(--pmax-gray-500);font-size:13.5px}
  textarea{resize:vertical;min-height:90px;line-height:1.6}
  select{cursor:pointer}
  .radio-opts{display:grid;grid-template-columns:1fr 1fr;gap:8px;margin-top:2px}
  @media(max-width:520px){.radio-opts{grid-template-columns:1fr}}
  .radio-item{display:flex;align-items:flex-start;gap:10px;padding:11px 13px;border-radius:var(--radius-sm);border:1.5px solid var(--pmax-gray-200);background:var(--pmax-gray-100);cursor:pointer;transition:var(--transition);user-select:none}
  .radio-item:hover{border-color:var(--pmax-blue-light);background:var(--pmax-blue-pale)}
  .radio-item input[type="radio"]{display:none}
  .radio-dot{width:18px;height:18px;border-radius:50%;border:2px solid var(--pmax-gray-200);background:white;flex-shrink:0;margin-top:2px;transition:var(--transition);display:flex;align-items:center;justify-content:center}
  .radio-item.selected{border-color:var(--pmax-blue);background:var(--pmax-blue-pale)}
  .radio-item.selected .radio-dot{border-color:var(--pmax-blue);background:var(--pmax-blue);box-shadow:inset 0 0 0 3px white}
  .radio-content{display:flex;flex-direction:column;gap:2px}
  .radio-label{font-size:13px;font-weight:600;color:var(--pmax-dark)}
  .radio-sub{font-size:11.5px;color:var(--pmax-gray-500);line-height:1.4}
  .radio-item.selected .radio-label{color:var(--pmax-blue)}
  .budget-tiers{display:grid;grid-template-columns:repeat(3,1fr);gap:10px;margin-bottom:4px}
  @media(max-width:480px){.budget-tiers{grid-template-columns:1fr}}
  .tier-btn{padding:12px 8px;border-radius:var(--radius-sm);border:1.5px solid var(--pmax-gray-200);background:var(--pmax-gray-100);cursor:pointer;text-align:center;transition:var(--transition);font-family:'Be Vietnam Pro',sans-serif}
  .tier-btn:hover{border-color:var(--pmax-blue-light);background:var(--pmax-blue-pale)}
  .tier-btn.selected{border-color:var(--pmax-blue);background:var(--pmax-blue-pale)}
  .tier-value{font-size:12.5px;font-weight:700;color:var(--pmax-dark);margin-bottom:2px}
  .tier-label{font-size:11px;color:var(--pmax-gray-500)}
  .tier-btn.selected .tier-value{color:var(--pmax-blue)}
  .duration-opts{display:flex;flex-wrap:wrap;gap:8px}
  .dur-btn{padding:8px 14px;border-radius:99px;border:1.5px solid var(--pmax-gray-200);background:var(--pmax-gray-100);font-family:'Be Vietnam Pro',sans-serif;font-size:13px;font-weight:600;color:var(--pmax-gray-700);cursor:pointer;transition:var(--transition)}
  .dur-btn:hover{border-color:var(--pmax-blue-light);color:var(--pmax-blue);background:var(--pmax-blue-pale)}
  .dur-btn.selected{border-color:var(--pmax-blue);background:var(--pmax-blue);color:white}
  .vat-opts{display:flex;gap:8px;flex-wrap:wrap}
  .vat-btn{padding:8px 16px;border-radius:99px;border:1.5px solid var(--pmax-gray-200);background:var(--pmax-gray-100);font-family:'Be Vietnam Pro',sans-serif;font-size:13px;font-weight:600;color:var(--pmax-gray-700);cursor:pointer;transition:var(--transition)}
  .vat-btn:hover{border-color:var(--pmax-blue-light);color:var(--pmax-blue);background:var(--pmax-blue-pale)}
  .vat-btn.selected{border-color:var(--pmax-blue);background:var(--pmax-blue);color:white}
  /* NDA badge */
  .nda-badge{display:inline-flex;align-items:center;gap:6px;background:#FFF3E8;border:1.5px solid #FF6B00;border-radius:var(--radius-sm);padding:8px 13px;font-size:12px;font-weight:600;color:#B84D00;margin-top:2px}
  .nda-badge::before{content:'🔒';font-size:13px}
  .nav-row{display:flex;justify-content:space-between;align-items:center;margin-top:6px;padding-top:18px;border-top:1px solid var(--pmax-gray-100)}
  .btn{display:inline-flex;align-items:center;gap:7px;padding:11px 22px;border-radius:var(--radius-sm);font-family:'Be Vietnam Pro',sans-serif;font-size:14px;font-weight:600;cursor:pointer;border:none;transition:var(--transition)}
  .btn-ghost{background:transparent;color:var(--pmax-gray-500);border:1.5px solid var(--pmax-gray-200)}
  .btn-ghost:hover{border-color:var(--pmax-gray-500);color:var(--pmax-dark)}
  .btn-primary{background:var(--pmax-blue);color:white}
  .btn-primary:hover{background:var(--pmax-blue-light);box-shadow:0 4px 20px rgba(0,51,160,0.28)}
  .btn-primary:active{transform:scale(0.98)}
  .btn-submit{background:var(--pmax-blue);color:white;padding:13px 32px;font-size:15px;border-left:4px solid var(--pmax-orange)}
  .btn-submit:hover{background:var(--pmax-blue-light);box-shadow:0 4px 24px rgba(0,51,160,0.3)}
  .btn-submit:disabled{opacity:0.6;cursor:not-allowed}
  .field.error input,.field.error textarea,.field.error select{border-color:#EF4444!important;background:#FFF5F5!important}
  .field.error .radio-opts,.field.error .budget-tiers,.field.error .duration-opts,.field.error .vat-opts{outline:2px solid #EF4444;outline-offset:4px;border-radius:var(--radius-sm)}
  .field-err{font-size:12px;color:#EF4444;font-weight:500;display:block;margin-top:4px}
  .summary-section{margin-bottom:22px}
  .summary-section h3{font-size:12px;font-weight:700;text-transform:uppercase;letter-spacing:0.8px;color:var(--pmax-blue);margin-bottom:10px;padding-bottom:8px;border-bottom:1px solid var(--pmax-gray-200);display:flex;justify-content:space-between;align-items:center}
  .btn-edit-section{font-size:11px;font-weight:600;color:var(--pmax-blue);background:var(--pmax-blue-pale);border:1px solid rgba(0,51,160,0.18);border-radius:99px;padding:3px 10px;cursor:pointer;font-family:'Be Vietnam Pro',sans-serif;text-transform:none;letter-spacing:0;transition:var(--transition);white-space:nowrap}
  .btn-edit-section:hover{background:var(--pmax-blue);color:white}
  .summary-row{display:flex;gap:12px;padding:7px 0;border-bottom:1px solid var(--pmax-gray-100);font-size:13px}
  .summary-row:last-child{border-bottom:none}
  .summary-key{width:190px;flex-shrink:0;color:var(--pmax-gray-500);font-weight:500}
  .summary-val{color:var(--pmax-dark);font-weight:500;flex:1}
  .summary-empty{color:#b0bad0;font-style:italic;font-weight:400}
  .success-card{display:none;background:var(--pmax-white);border-radius:var(--radius);border:1px solid var(--pmax-gray-200);padding:56px 32px;text-align:center;box-shadow:var(--shadow-card);animation:fadeUp 0.4s ease}
  .success-card.show{display:block}
  .success-icon{width:72px;height:72px;background:#DCFCE7;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:32px;margin:0 auto 20px}
  .success-title{font-size:23px;font-weight:800;color:var(--pmax-dark);margin-bottom:10px}
  .success-sub{font-size:14px;color:var(--pmax-gray-500);line-height:1.7;max-width:400px;margin:0 auto 28px}
  .success-detail{background:var(--pmax-gray-100);border-radius:var(--radius-sm);padding:16px 20px;text-align:left;max-width:480px;margin:0 auto;font-size:13px;color:var(--pmax-gray-700);line-height:1.8}
  .site-footer{max-width:780px;margin:0 auto;padding:24px;text-align:center;font-size:12px;color:var(--pmax-gray-500)}
  .site-footer a{color:var(--pmax-blue);text-decoration:none}
</style>
</head>
<body>

<header class="site-header">
  <div class="header-inner">
    <a class="logo" href="#"><img src="data:image/png;base64,/9j/4AAQSkZJRgABAQAAAQABAAD/4gHYSUNDX1BST0ZJTEUAAQEAAAHIAAAAAAQwAABtbnRyUkdCIFhZWiAH4AABAAEAAAAAAABhY3NwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAQAA9tYAAQAAAADTLQAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAlkZXNjAAAA8AAAACRyWFlaAAABFAAAABRnWFlaAAABKAAAABRiWFlaAAABPAAAABR3dHB0AAABUAAAABRyVFJDAAABZAAAAChnVFJDAAABZAAAAChiVFJDAAABZAAAAChjcHJ0AAABjAAAADxtbHVjAAAAAAAAAAEAAAAMZW5VUwAAAAgAAAAcAHMAUgBHAEJYWVogAAAAAAAAb6IAADj1AAADkFhZWiAAAAAAAABimQAAt4UAABjaWFlaIAAAAAAAACSgAAAPhAAAts9YWVogAAAAAAAA9tYAAQAAAADTLXBhcmEAAAAAAAQAAAACZmYAAPKnAAANWQAAE9AAAApbAAAAAAAAAABtbHVjAAAAAAAAAAEAAAAMZW5VUwAAACAAAAAcAEcAbwBvAGcAbABlACAASQBuAGMALgAgADIAMAAxADb/2wBDAAUDBAQEAwUEBAQFBQUGBwwIBwcHBw8LCwkMEQ8SEhEPERETFhwXExQaFRERGCEYGh0dHx8fExciJCIeJBweHx7/2wBDAQUFBQcGBw4ICA4eFBEUHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh4eHh7/wAARCACUAQ4DASIAAhEBAxEB/8QAHQABAAICAwEBAAAAAAAAAAAAAAcIBgkDBAUCAf/EAEwQAAECBQMBBAQGDQsEAwAAAAECAwAEBQYRBxIhMQgTQVEUImGBFRYyQnGRFyM1UlRVc5KTlKGx0RgkM1NWV2JygpXSCTRD4qKywf/EABwBAQAABwEAAAAAAAAAAAAAAAABAgMEBQYHCP/EADgRAAEDAgQCBwYGAwADAAAAAAEAAhEDBAUSITEGQQcTIlFhcYEyQpGhscEUcoLC0fAVUmIIsuH/2gAMAwEAAhEDEQA/ALlwhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQjCtZq6aLZMy0y5smp/8AmzWDggK+WofQnPPgSI9HTSu/GGz5KdcVumEJ7l/z3p4J9/X3xZi+pG6NrPaAlZA4bWFkL33S7L8t/LceiySEIReLHpCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCBIAyeBHT+FqX+MpL9On+MTNY52wRdyEdP4Wpf4yk/06f4w+FqX+MpP9On+MTdU/uKhIXchHT+FqX+MpP9On+Mc8tNS0yCZeYZeA692sKx9UQNNwEkKMrlhCESIkIRG1q6jNVfVysWuHU+hto7uTV9+61nvQP24/yExdW1lWuW1H0xIYJPl/fkCrevdUqDmNeYLjA81JMIRjWqFzt2fYtUrqlIDzLJTLJV0W8rhAx488n2AxZveGNLnbBX9tb1LmsyjSEucQB5nRQ5rdXjVrxck2nCZanAsAA8Fz55+vA9xjv6BV/wBAuN2iPuYYqCSWsngOpGf2pB+oecRPQp9dSpjU26ta3l571auql/OUfpPPvjILYQ4a3LPtKKVSriXwoeBSQU/tA/bHIXYtUoYib1+4Oo8No+C7Xd4NSpYa6wds0RPiOfx1VsYR1KPPN1KmS881wl5AVjyPiPrjtx12nUbUYHtMg6hcPewscWu3CQj5cWhttTji0oQkFSlKOAAOpJjq/C1L/GUn+nT/ABiq1jnbBSruQjglpyUmioS00w8U8qDbgVj6o54gQQYKJCEcczMS8sgOTD7TKCcBTiwkE+XMACTARckI6fwtS/xlJ/p0/wAY5Zadk5lRTLTbDykjJDbgUQPdExpvAkhJXPCEIkRIR8PvMy7ZdfdbabHVS1BI+sx1vhal/jKT/Tp/jEwY52oCSu5COGWnJSaKhLTTD5T8ru3ArH04jmiBBBgokIQiCJCEIIuCo/c+Z/JK/cY1QpmH0gAPugDgALPEbXqj9z5n8kr9xjU7HZ+iQAtu5/4/esdf+76rl9Jmfwh388w9Jmfwh388xZvsO2ja1zyVyKuK3qXVlMONBozkqh0oBBzjcDiLK/Ym0w/u/tn/AG1r/jGw430g2eE3r7OpRc4tjURGoB+6pU7R1RocCtZ/pMz+EO/nmOeSqtUkphExJVKclnm1bkOMvqQpJ8wQcgxsoOk2mBGPsf2z/trX8Irl2udELYta2E3paEoaahEwlqck0KUpshfRaQSduD1A49giXCOkPDcUum2jqTml+gmCJ7j5pUtHsbmlfPZt7R9WbrMlaWoM6Z2TmVJYlaq8ftrKzwkOq+ek9N55B5JI6XEjUtGzXQ2uTFyaR2zWZtRVMPyCA6oqyVKT6hJPmduffGn9JXDltYOp31q0NDyQ4DadwQOU6yrizrF0tcu3qtcnxWsWo1RtYTNFHcynn3q+En245VjySYqJQqpN0atydYk1n0mUfS8glR9Yg5IJ8iMg+YJiQ+01fcvUtQ2rGlngpNMlxMPgcgvL8D5EII/OiL4ueFsJ/C4fmqt1q6/pO3y19VoXFV5UdfBo0DAI895+3oryUKpStZo0nVZNW6Xm2Uut56gEZwfaOhiuHbBuwTNVkbRlXcolR6TNbVfPUPVSfoHPvjPtFK83b2l80qtvFLdOYcnQknkM8q2gHxz4eagIqjdFYmrguKfrc6ol+dfU8oFRO3J4SCfADAHsEcT4sAsar7VpnU/DkvRHQ3bU8bq/5XdtMR+vUEemvyK9Sw5/upxcgs+q8NyP8wHP1j90TBbMt3Mh3qhhb3PPl4REGldvzVz3/SKPKlaO9mEqecT/AONpPrLV+aDjPBJA8YnypSDlLn3qe4kBUuvZwMAgdCPYRgxx7iO2qMY2sB2XGCfEfz9l0ziuvSZcig09ojMR4TE/3uWeaS1TKJikOL5T9taB8vnAe/n3xn8QTQ6g5S6vLT7eSWXAVAfOT0UPeMiJzZdbeYQ82oKbWkKSfMGN44GxT8XY/h3HtU9PQ7fcegXF+IrPqbjrRs768/5UCdt29hb+mSbalX9k9XnO6UEqwoS6SCv24J2p+gkeMUZ9Jmfwh388xJfaevgXzq1UpuWf72myB9CksKykpQSFLHOPWVk5HUYiPKbSqjUmJ5+Qk3ZhuQl/SZpSBnumtyUFZ9mVp+vPQGPaXBuENwjCKbKujndp097ogeggea0S4qdZUMKRuzFfrtlau0uam5lYptRUJCe3qyEocICV8njavaony3DxjYtGpZJKSCCQRyCPCNj3ZpvdN9aTUufdeDk/Jp9DnRnJ7xAAyeT1Tg8885jR+lTBo6rEaY/5d9Wn6j4K5sam7CpLjyLytuk3bbU7b1blg/IzjexY6KSeqVpPgpJAIPgQI9eEcepVH0niowwRqCORWQInQrWdrHY9d02vSYoFRffdZ/pJOa5CZhonhQ9vgR4GOjpjfVasK9pC5qZMOKcllbXmVLOyYZVje2rzBA9xCT1Ai/uvOmNO1Psp2lPFEvU5fLtOmynJacx8k/4FdD9fURrnuKj1G365OUWryq5Wek3S081sMKRuQPVdU4BnOAc4HWLu24gsX3VY3bszHPpwYJLWtzGRpoA4iRzBMBQNJ2UZe4qPNVZiVXeulMrWJavVKmTFurVMydKecS++oM5SfUUknCsE89AY7eqkvQ6X2f5edt+m3PRZSauSW9Il6hMPmbwCUKxlalAKSOADzEh3dpNXqhXbQrtu3q1Q6jbVMVIturpaZkO7kbFK2qWAOM8c9esc9e0zu25rLRQrqv5mqTbVYl6g1OJpCGQltrB7rYhfOTk7s+PSJqeNWTRaHroaw9oS//dx9nLlOhBmZ5RooGm7tafTuWEaMLkntcnUadfGNi2JWmrbrrFXeeKUzBOWQhDyitK/HJGMbsRYyMHbsJyT1gVf1JqqZRqdkvRKtTyxuTNlP9G4FBQ2rScclKsjI4zkZxGqY9e0r2tTq0jIyNBmS6dZzEgZjOxHuxzBVek0tBBSEIRg1VSEIQRIQhBEhCEEXBUfufM/klfuManY2xVH7nzP5JX7jGp2O0dEns3f6P3rHX/u+qtF2GrUti5JK5FXDbtJq5ZcaDRnZNt7ZkHO3cDj3RZf7Fumf93tqf7Qx/xiAf8Ap7/9jdP5Vn9xi10alx1fXVLHa7WVHAaaAke6FXtmtNISFh/2LdM/7vbU/wBoY/4x6FEsezKHMGZo1pUKmvnguStPaaUfelIMZBCNPfiF09pa6q4jzP8AKuAxo5JFA+2nRKtTNa5uoT77j8rUmG3pJauiEJSElsfQQT/qi/kQZ20LJFzaUvVuWZ3T1BUZoEDks9HB9AHrf6TG08BYq3DsZYX+zU7B8JiPmB6KhdU89MxyVH7Nt+fuq6qZblMTum6jMoYbJBITuPKjjwSMk+wGNl7lqycpYTFsUxsIZkpZDUsMDOUDjPtODk+0xV3sGWKJut1G/Z5nLckkykhuH/kUPtixkeCcJBB+coRcaM70lY6a2JMtKR0o6n8x1+QgfFWYsad1avpVhLXgg+R0UDKBSopUCCDgg+EZXptQpeerCKzMspWaeo+jKI+S4pJSSP8AST9fsjragv0yFfW6hOGZr7YjAwAfnD6+ffEiWvTvgqiS8oQA4E7nMHPrHrGrYndsfZiPf+2vyK45wLw9c23EdQOJH4eZI0nMC0ejmknxGh3XpwhCNXXeFiepNwyGn1gV66S00FS7K30NqOA8+obUJP0q2j2AkxrJqU7NVKozNQnnlPzU08t591XVa1EqUo+0kkxart73uVO0qwpN31U/z6eAPjyG0n/5GKrUuRmqnU5WmyLSnpqbeQww2nqta1BKQPpJEegejTBmYdhZu3iDV18mjb46n1Cxd9VNSpEzC7Nu16tW5UhUqDVJumTgQUB+VdLa9p6jI5wYyX7LmqH9v7k/3Bz+MW1pfZR01RTJVFQNYdnEspEwtE5hKnMDcQNvAznEdn+SppT/AFdb/Xv/AFiS46QOG6z81WmXHvLAfqVAWlYDQ/NUzruol916lu0utXfW6hIvY7yXmJxa0LwQRkE4OCAYxeL6fyVNKf6ut/r3/rFdO1VpJIaZV6mvUATSqLUGSEl9e9SHkn1huwOoIMZbAeMcFv7gWdm0sLpIGUNBgeB3j6KSrb1GjM5SV2Cb59ep6fzr3gZ6nhR+gOoH1hWP83lFto1a6dXNOWbfNHueRUQ9T5pLpH36Oi0H2KQVJPsMbOWa5S3LcRcRnGm6YqVE2ZhagEpa27txPhgRzbpLwQ2uJNuqQ7Nb/wBhofjofOVeWdTMzKeS8/Ua8KPYloT1y1t0plpVGUtpxveWfktpB6qJ4/b0Ea3tT73rOoF4Tdx1pz7a8drLKTlDDQ+S2n2Dz8TkxmHaT1amdTrs2ya3W7ekFFMgyrjeehdUPM+GeQPfGIaW2RV9Qbzk7ao6Ptjytz7yh6jDQPrOK9gH1kgeMb3wZw1S4esnX17AqESSfcbvHn3/AA5a2txWNV2VuyznsxaQP6l3SJ2poU3bVNcSqdXkgzCuoZSfb84+A6ckR6fax0e+IFw/GChS2226k6diEA4lHjklv2JOCU+8eEXYsG1KRZNqSVuURgNSkqjGces4r5y1eaieTHPeNuUm7bZnrerkqmZkJ1otuoPUeIUk+CgQCD4ECNIf0j3JxoXQn8OOzl/57/zc/lsrkWY6vLzWrejVKeo9VlarTJpyVnZR1LzDzZwpC0nIIjYr2fdUpDU+zUToKWaxKANVGW+9Xj5af8Kuo948IojrFp9VdNr1mbfqOXWf6STmQnCZhknhQ9vgR4GOvpTfVY08vOTuOjuqy2rZMsE+pMsk+s2oe3wPgQD4R0XijALfijDm1rYgvAlju+eR8D8j6q0oVTQfB25rZ/CPDsS6qRelrSVxUR8PSk0jcAflNq8UKHgQeDHuR5vq0n0ahp1BDgYIPIhZcEESEhCEU1FIQhBFxzLffSzrQON6CnPlkRUlPY4mdo3XwyVY5xInGfzot1CM3g/EWIYMHiyflzROgO0xuD3lU6lJlT2gol7O+j7ulDNWacraKoJ9SFApYLezbn2nPWJagSB1IGeIRY4hiFxiNw65uXS924gDYRyUzGBggJCEIslMkcU3LsTco9KTTSHmHm1NutrGUrSoYII8iDHLCIgkGQixvTSzqZYVnSds0kqVLyxUe8WAFuKUokqVjjPQe6MkhCKlevUuKrqtUy5xknvJUAABAXQqtLl6i9JuvjPor3epHnx0PvwfdHfhCJC9xABOgVKnb0qdR9RrYc6JPfAgfAJCEIlVZVhv3svVi8bxqlzVO+WfSahMKd2iSOG0dEIHrchKQlOfHEeno92Y5ex9QJC6ajcLdWTIBa2JcSuwd8RhKyST8nJI9u0+EWLhG1VONMZfbG1NWGEZYDWjSIjQdyoC2p5s0apCEI1VV0jBNctOZTU6xnLeemhJTCH0Pys13e/ulJPPHiCkqGM+R8IzvI3bcjOM4hFxaXdazrsr0TDmmQfFQc0OEFVG/kcTH9uGv1E/8okCp6J3lPaSU/TY3+y1TJVZLriJM75hvOUNK9bhCfLxwM9InmEbHccbYzclhrVA7IcwlrdD37eKoi2pt2CqN/I4mP7cNfqJ/wCUTloNpNSdK7eek5Z1M7U5te6cni3tU4B8lAHOEjy8yTEjwihifF2L4pQNvc1pYdYgCY74AUWW9NhloSEIRrarKPtddLaVqlaiaXNuiSqEusOSU6G9xaPzkkcZSocEZ64PhED/AMjiY/tw1+on/lFuYRseF8W4thdD8Pa1YZMxAO/dIKovoU3mXBQtoHo7celVUmEtXi1UqLOJ/nEiuVUnCwPVcQdx2q8DxyOvIGJphCMXiWJXGJVzcXJBedyABPnAHxVRjAwQEhCEWCmSEIQRfLqEuNqbVnaoEHBxwYrV9jS2B2kE2WF1r4E+LSp7uPhiZz3weSndu37uhxjOIsvGF/EZX2ZxqJ8JjaKMaX6F3HPLgX3m/d7MY2++M7gmJuseuioW5mECJ9r3due8HkqVRmaNFHCLVltS9Xr5ptx1OsJkaCmXkqWzJzzjAl97KVqd9U4UvKs+tkcDIMY7R5VN+9lRy8bjmqi/XKJSJ70SaannWiVNpKkqWEKAWQUj5QPSJKu/S6vzF4VS57Hvt+1ZqtMoZqiDIpmkOlKdqXEblDu1hOBkeQ6ePsyem1OpmjM3ptSZxxlh+mvyQm3kBa9zqFAuKSMA8qzjjpjMZ443b06VEsq6g0oABBYGtIqco7ZM9knNudVS6skmR3+vcsV0ulLd090U+yERPOPu0JudnjMT7r3eqS2VBKQtRCSpRxxjkiPA7L9RuKlV+boF3VFU5OXHIIuSWUpROwuKPetDJIGMtqwMfL6cRnVz6XvVvSSj6dmvmXk5VMs1PPplyVTTLRGUAbvU3Y65OOOsdBrQ63aLeFvXNZbztEmqVMlUwl55+bTMy6klKmQHHcI4JwRnBxwcRT/yWH1qFy24qkvrF0HKTAbrT1Ook6aA6RMKOR4LYGg/pX32Zn3n7Srqn3nHVJuOoIBWoqIAeOBz4CO92m3npfQi6npd1xl1EqkpWhRSpJ71HII6Rj1F0q1It1VRYtnViXp0hOT784JdVvNvFCnVlRG5TmT1jP8U60Hb16dKmpaqKI03KgwlpU0Wd4SQpKidmRnO3pkdYsbitZsxmneNrNcwva4wHS0AgmQWj5TspgHdWWxrCrBcGpt0TegadPkekpu2Ul91QdSs7kU5pkPh7f8A4kFCc+7xiS7+qlQmtCLEs6lz7svV7sRIyKZkKJU01tSt50kEHhIyfMZjP6tphSJ2zJ2lNplWa1OW+KG5VxL5WWw2EZ27umRnbnyGY8Kc0RptaqtvLuiprqdLoNFTT5WTZDssrvhtCn+8bcCuQnG32nkxmTjeEVCx4GTI91QiJJcW6QNBlzRDSRAGpVPq6gnnpCwmvXNUah2Oq+3NTS2q5QgmlTq2nvXS6xMtoyFDnkAc+MePpm7T3tULMY05F1sTTUuHrmRUn3xLql1N/K2PKySV/JKRjOIkCb0FlWLfvS26BX3KdRblbYUiVeaXMGUfbWlSnAtTm5e8JGQTkefhGSTumrybytK66RWkSNRokomQnsyu9FQlcAKQcKBSeCUnKgDjg4ib/M4ZSoVqVF+lQ1HAQQBmptgObBmHZgIJykA6hOreSCeUfVVyF7VdNXvSxkVGo0yQq97vS1SrpypuQlVuqQGkKz6qlbSPAAHr1iR9f6dSKDXdOKCZKuTlEbVMMuydNmHPSZhIaJHrJUFKO4BROfAxm9K0ap7dtX7QKvUhPyt3VOYqG5Mt3apRThyjGVHcpCsKB4yR0jp1fSi752nWc4xqEzLVy10uIaqJpAd74KQUAlCnMZCSQTk568RWfjmG1LplSm/IG5gdHdomnAfIaSCHdnbQQWjdQFJ4aQR/ZX1Ylj2NctlTMuzQrrpUkucDq2KlUJlt8rQnAUFd6VBOD0zg+URrpFb0iezXdV7rmKm5XU0msy4mHKg8pIQltwJwgq2ggJHOMxYCwaNd1JlJpu7bwbuR51YLLiKaiUDSccjCSd3POYx2z9LV2/orVtOVVtMyqoS86z6cJXYG/SAsZ7vec7d333OPCMTTxsU21abq5INSmRq8gtGbPq4Ax7MyATA0MKc05gxyKhK7H7vc090ZXaU5MGu909MML2MBSf51raalOKzjZ7ucRkOt91V4aqruaiT626Tp6uTNSl0KI9K9Ic2vIx0ylsjPXAVnjEWBs+jqt+1KZQzMCYVIyqGO+CNu/aMZ25OPozEXU/s8WpNU+qu3c/M1quVWYfmJmfZmJiVRucJIAZS6U4TkAA56CLyjxDh9S8dXuZytlo0zucHO7Uk5QAGy0DduaQDClNJ4bDVjHaLnqNMauafGruVaat+bkptyYama3+8fT3alNkJZIWcK2njwznjMdnQigy17UG6JV16sv6ezFRbcoAmZ91MyCkfbftiVbwjd0BOeuYzC39J6hI3FYNZqF0InnLRk5iUI9DKTNhxpbaTkuHZtCvbnHhHv6aWI5Y9SuBEnVUvUSpzpnZSnlgpMkt/9Ikr3EFJPIASnHtihdYxa0sNFrbVSXsaIOsSKrjIECH5cpzf6kt3UW03F+Zw/sKOeznZdF72t3CtdUdqFJrtRk5NTtSfWhDSVLaSkoKtqsJJ5IJzz1iI9P76r9E0Nrts3ROvGWrVGmpy3p9bhKu8QPtjBXnIVxuT7xnoItVpxZqrQp9ZlFVETnwlVJqobgzs7vvllWzqc4zjPGfIRg09oLTqjobJ6b1GrpdmpBwvSdUTK4LLmc52buQQSkjdznPUCLu24gsX3VY3bszHPpwYJLWtzGRpoA4iRzBMBQNJ2UZe4qPNVZiVXeulMrWJavVKmTFurVMydKecS++oM5SfUUknCsE89AY7eqkvQ6X2f5edt+m3PRZSauSW9Il6hMPmbwCUKxlalAKSOADzEh3dpNXqhXbQrtu3q1Q6jbVMVIturpaZkO7kbFK2qWAOM8c9esc9e0zu25rLRQrqv5mqTbVYl6g1OJpCGQltrB7rYhfOTk7s+PSJqeNWTRaHroaw9oS//dx9nLlOhBmZ5RooGm7tafTuWEaMLkntcnUadfGNi2JWmrbrrFXeeKUzBOWQhDyitK/HJGMbsRYyMHbsJyT1gVf1JqqZRqdkvRKtTyxuTNlP9G4FBQ2rScclKsjI4zkZxGqY9e0r2tTq0jIyNBmS6dZzEgZjOxHuxzBVek0tBBSEIRg1VSEIQRIQhBEhCEEXBUfufM/klfuManY2xVH7nzP5JX7jGp2O0dEns3f6P3rHX/u+qtF2GrUti5JK5FXDbtJq5ZcaDRnZNt7ZkHO3cDj3RZf7Fumf93tqf7Qx/xiAf8Ap7/9jdP5Vn9xi10alx1fXVLHa7WVHAaaAke6FXtmtNISFh/2LdM/7vbU/wBoY/4x6FEsezKHMGZo1pUKmvnguStPaaUfelIMZBCNPfiF09pa6q4jzP8AKuAxo5JFA+2nRKtTNa5uoT77j8rUmG3pJauiEJSElsfQQT/qi/kQZ20LJFzaUvVuWZ3T1BUZoEDks9HB9AHrf6TG08BYq3DsZYX+zU7B8JiPmB6KhdU89MxyVH7Nt+fuq6qZblMTum6jMoYbJBITuPKjjwSMk+wGNl7lqycpYTFsUxsIZkpZDUsMDOUDjPtODk+0xV3sGWKJut1G/Z5nLckkykhuH/kUPtixkeCcJBB+coRcaM70lY6a2JMtKR0o6n8x1+QgfFWYsad1avpVhLXgg+R0UDKBSopUCCDgg+EZXptQpeerCKzMspWaeo+jKI+S4pJSSP8AST9fsjragv0yFfW6hOGZr7YjAwAfnD6+ffEiWvTvgqiS8oQA4E7nMHPrHrGrYndsfZiPf+2vyK45wLw9c23EdQOJH4eZI0nMC0ejmknxGh3XpwhCNXXeFiepNwyGn1gV66S00FS7K30NqOA8+obUJP0q2j2AkxrJqU7NVKozNQnnlPzU08t591XVa1EqUo+0kkxart73uVO0qwpN31U/z6eAPjyG0n/5GKrUuRmqnU5WmyLSnpqbeQww2nqta1BKQPpJEegejTBmYdhZu3iDV18mjb46n1Cxd9VNSpEzC7Nu16tW5UhUqDVJumTgQUB+VdLa9p6jI5wYyX7LmqH9v7k/3Bz+MW1pfZR01RTJVFQNYdnEspEwtE5hKnMDcQNvAznEdn+SppT/AFdb/Xv/AFiS46QOG6z81WmXHvLAfqVAWlYDQ/NUzruol916lu0utXfW6hIvY7yXmJxa0LwQRkE4OCAYxeL6fyVNKf6ut/r3/rFdO1VpJIaZV6mvUATSqLUGSEl9e9SHkn1huwOoIMZbAeMcFv7gWdm0sLpIGUNBgeB3j6KSrb1GjM5SV2Cb59ep6fzr3gZ6nhR+gOoH1hWP83lFto1a6dXNOWbfNHueRUQ9T5pLpH36Oi0H2KQVJPsMbOWa5S3LcRcRnGm6YqVE2ZhagEpa27txPhgRzbpLwQ2uJNuqQ7Nb/wBhofjofOVeWdTMzKeS8/Ua8KPYloT1y1t0plpVGUtpxveWfktpB6qJ4/b0Ea3tT73rOoF4Tdx1pz7a8drLKTlDDQ+S2n2Dz8TkxmHaT1amdTrs2ya3W7ekFFMgyrjeehdUPM+GeQPfGIaW2RV9Qbzk7ao6Ptjytz7yh6jDQPrOK9gH1kgeMb3wZw1S4esnX17AqESSfcbvHn3/AA5a2txWNV2VuyznsxaQP6l3SJ2poU3bVNcSqdXkgzCuoZSfb84+A6ckR6fax0e+IFw/GChS2226k6diEA4lHjklv2JOCU+8eEXYsG1KRZNqSVuURgNSkqjGces4r5y1eaieTHPeNuUm7bZnrerkqmZkJ1otuoPUeIUk+CgQCD4ECNIf0j3JxoXQn8OOzl/57/zc/lsrkWY6vLzWrejVKeo9VlarTJpyVnZR1LzDzZwpC0nIIjYr2fdUpDU+zUToKWaxKANVGW+9Xj5af8Kuo948IojrFp9VdNr1mbfqOXWf6STmQnCZhknhQ9vgR4GOvpTfVY08vOTuOjuqy2rZMsE+pMsk+s2oe3wPgQD4R0XijALfijDm1rYgvAlju+eR8D8j6q0oVTQfB25rZ/CPDsS6qRelrSVxUR8PSk0jcAflNq8UKHgQeDHuR5vq0n0ahp1BDgYIPIhZcEESEhCEU1FIQhBFxzLffSzrQON6CnPlkRUlPY4mdo3XwyVY5xInGfzot1CM3g/EWIYMHiyflzROgO0xuD3lU6lJlT2gol7O+j7ulDNWacraKoJ9SFApYLezbn2nPWJagSB1IGeIRY4hiFxiNw65uXS924gDYRyUzGBggJCEIslMkcU3LsTco9KTTSHmHm1NutrGUrSoYII8iDHLCIgkGQixvTSzqZYVnSds0kqVLyxUe8WAFuKUokqVjjPQe6MkhCKlevUuKrqtUy5xknvJUAABAXQqtLl6i9JuvjPor3epHnx0PvwfdHfhCJC9xABOgVKnb0qdR9RrYc6JPfAgfAJCEIlVZVhv3svVi8bxqlzVO+WfSahMKd2iSOG0dEIHrchKQlOfHEeno92Y5ex9QJC6ajcLdWTIBa2JcSuwd8RhKyST8nJI9u0+EWLhG1VONMZfbG1NWGEZYDWjSIjQdyoC2p5s0apCEI1VV0jBNctOZTU6xnLeemhJTCH0Pys13e/ulJPPHiCkqGM+R8IzvI3bcjOM4hFxaXdazrsr0TDmmQfFQc0OEFVG/kcTH9uGv1E/8okCp6J3lPaSU/TY3+y1TJVZLriJM75hvOUNK9bhCfLxwM9InmEbHccbYzclhrVA7IcwlrdD37eKoi2pt2CqN/I4mP7cNfqJ/wCUTloNpNSdK7eek5Z1M7U5te6cni3tU4B8lAHOEjy8yTEjwihifF2L4pQNvc1pYdYgCY74AUWW9NhloSEIRrarKPtddLaVqlaiaXNuiSqEusOSU6G9xaPzkkcZSocEZ64PhED/AMjiY/tw1+on/lFuYRseF8W4thdD8Pa1YZMxAO/dIKovoU3mXBQtoHo7celVUmEtXi1UqLOJ/nEiuVUnCwPVcQdx2q8DxyOvIGJphCMXiWJXGJVzcXJBedyABPnAHxVRjAwQEhCEWCmSEIQRfLqEuNqbVnaoEHBxwYrV9jS2B2kE2WF1r4E+LSp7uPhiZz3weSndu37uhxjOIsvGF/EZX2ZxqJ8JjaKMaX6F3HPLgX3m/d7MY2++M7gmJuseuioW5mECJ9r3due8HkqVRmaNFHCLVltS9Xr5ptx1OsJkaCmXkqWzJzzjAl97KVqd9U4UvKs+tkcDIMY7R5VN+9lRy8bjmqi/XKJSJ70SaannWiVNpKkqWEKAWQUj5QPSJKu/S6vzF4VS57Hvt+1ZqtMoZqiDIpmkOlKdqXEblDu1hOBkeQ6ePsyem1OpmjM3ptSZxxlh+mvyQm3kBa9zqFAuKSMA8qzjjpjMZ443b06VEsq6g0oABBYGtIqco7ZM9knNudVS6skmR3+vcsV0ulLd090U+yERPOPu0JudnjMT7r3eqS2VBKQtRCSpRxxjkiPA7L9RuKlV+boF3VFU5OXHIIuSWUpROwuKPetDJIGMtqwMfL6cRnVz6XvVvSSj6dmvmXk5VMs1PPplyVTTLRGUAbvU3Y65OOOsdBrQ63aLeFvXNZbztEmqVMlUwl55+bTMy6klKmQHHcI4JwRnBxwcRT/yWH1qFy24qkvrF0HKTAbrT1Ook6aA6RMKOR4LYGg/pX32Zn3n7Srqn3nHVJuOoIBWoqIAeOBz4CO92m3npfQi6npd1xl1EqkpWhRSpJ71HII6Rj1F0q1It1VRYtnViXp0hOT784JdVvNvFCnVlRG5TmT1jP8U60Hb16dKmpaqKI03KgwlpU0Wd4SQpKidmRnO3pkdYsbitZsxmneNrNcwva4wHS0AgmQWj5TspgHdWWxrCrBcGpt0TegadPkekpu2Ul91QdSs7kU5pkPh7f8A4kFCc+7xiS7+qlQmtCLEs6lz7svV7sRIyKZkKJU01tSt50kEHhIyfMZjP6tphSJ2zJ2lNplWa1OW+KG5VxL5WWw2EZ27umRnbnyGY8Kc0RptaqtvLuiprqdLoNFTT5WTZDssrvhtCn+8bcCuQnG32nkxmTjeEVCx4GTI91QiJJcW6QNBlzRDSRAGpVPq6gnnpCwmvXNUah2Oq+3NTS2q5QgmlTq2nvXS6xMtoyFDnkAc+MePpm7T3tULMY05F1sTTUuHrmRUn3xLql1N/K2PKySV/JKRjOIkCb0FlWLfvS26BX3KdRblbYUiVeaXMGUfbWlSnAtTm5e8JGQTkefhGSTumrybytK66RWkSNRokomQnsyu9FQlcAKQcKBSeCUnKgDjg4ib/M4ZSoVqVF+lQ1HAQQBmptgObBmHZgIJykA6hOreSCeUfVVyF7VdNXvSxkVGo0yQq97vS1SrpypuQlVuqQGkKz6qlbSPAAHr1iR9f6dSKDXdOKCZKuTlEbVMMuydNmHPSZhIaJHrJUFKO4BROfAxm9K0ap7dtX7QKvUhPyt3VOYqG5Mt3apRThyjGVHcpCsKB4yR0jp1fSi752nWc4xqEzLVy10uIaqJpAd74KQUAlCnMZCSQTk568RWfjmG1LplSm/IG5gdHdomnAfIaSCHdnbQQWjdQFJ4aQR/ZX1Ylj2NctlTMuzQrrpUkucDq2KlUJlt8rQnAUFd6VBOD0zg+URrpFb0iezXdV7rmKm5XU0msy4mHKg8pIQltwJwgq2ggJHOMxYCwaNd1JlJpu7bwbuR51YLLiKaiUDSccjCSd3POYx2z9LV2/orVtOVVtMyqoS86z6cJXYG/SAsZ7vec7d333OPCMTTxsU21abq5INSmRq8gtGbPq4Ax7MyATA0MKc05gxyKhK7H7vc090ZXaU5MGu909MML2MBSf51raalOKzjZ7ucRkOt91V4aqruaiT626Tp6uTNSl0KI9K9Ic2vIx0ylsjPXAVnjEWBs+jqt+1KZQzMCYVIyqGO+CNu/aMZ25OPozEXU/s8WpNU+qu3c/M1quVWYfmJmfZmJiVRucJIAZS6U4TkAA56CLyjxDh9S8dXuZytlo0zucHO7Uk5QAGy0DduaQDClNJ4bDVjHaLnqNMauafGruVaat+bkptyYama3+8fT3alNkJZIWcK2njwznjMdnQigy17UG6JV16sv6ezFRbcoAmZ91MyCkfbftiVbwjd0BOeuYzC39J6hI3FYNZqF0InnLRk5iUI9DKTNhxpbaTkuHZtCvbnHhHv6aWI5Y9SuBEnVUvUSpzpnZSnlgpMkv/9Ikr3EFJPIASnHtihdYxa0sNFrbVSXsaIOsSKrjIECH5cpzf6kt3UW03F+Zw/sKOeznZdF72t3CtdUdqFJrtRk5NTtSfWhDSVLaSkoKtqsJJ5IJzz1iI9P76r9E0Nrts3ROvGWrVGmpy3p9bhKu8QPtjBXnIVxuT7xnoItVpxZqrQp9ZlFVETnwlVJqobgzs7vvllWzqc4zjPGfIRg09oLTqjobJ6b1GrpdmpBwvSdUTK4LLmc52buQQSkjdznPUCLu24gsX3VY3bszHPpwYJLWtzGRpoA4iRzBMBQNJ2UZe4qPNVZiVXeulMrWJavVKmTFurVMydKecS++oM5SfUUknCsE89AY7eqkvQ6X2f5edt+m3PRZSauSW9Il6hMPmbwCUKxlalAKSOADzEh3dpNXqhXbQrtu3q1Q6jbVMVIturpaZkO7kbFK2qWAOM8c9esc9e0zu25rLRQrqv5mqTbVYl6g1OJpCGQltrB7rYhfOTk7s+PSJqeNWTRaHroaw9oS//dx9nLlOhBmZ5RooGm7tafTuWEaMLkntcnUadfGNi2JWmrbrrFXeeKUzBOWQhDyitK/HJGMbsRYyMHbsJyT1gVf1JqqZRqdkvRKtTyxuTNlP9G4FBQ2rScclKsjI4zkZxGqY9e0r2tTq0jIyNBmS6dZzEgZjOxHuxzBVek0tBBSEIRg1VSEIQRIQhBFwVH7nzP5JX7jGp2Oz8qj9z5n8kr9xjU7HaOiT2bv9H71jr/3fVWi7Df8AJyMlI3P6ZOy0tsdZ2965lGeD0yY8bRm2Ke+KRN6dqLa7Y6hk+6FWvmtO4fDpkx6WjNsdN8Um701UW13R1DI90KtfNadw+HTJj0tGbY6b4pN3pqot7uihWqtNISlh/wBi3TP+721P9oY/4xAP+T3/AOxun8qz+4xa6NS46vrqljtdrKjgNNAEe6FXtmtNISFh/wBi3TP+721P9oY/4x6FEsezKHMGZo1pUKmvnguStPaaUfelIMZBCNPfiF09pa6q4jzP8quAxo5JFA+2nRKtTNa5uoT77j8rUmG3pJauiEJSElsfQQT/AKov5EGdtCyRc2lL1blmd09QVGaBA5LPRwfQB63+kxtPAWKtw7GWF/s1OwfCYj5geioXVPPTMclR+zbfn7quqmW5TE7puo1KGGiQSE7j8o48EjJPsBjZe5asnKWExbFMbCGZKWQ1LDAzlA4z7Tg5PtMVd7BlijbreMvWk1LQqt2UqScS4VHl84BgQcP0qAT9Yjaa+jTqLaRWbRrGn9SJWU0Cs1aa/UJBrYpxxpay4lp8pOW9oTggJznsZ8+p2y9Ov8A0YuBFXk56mT02taWQHXEY2MoAUDsAJGVeJPzR1IIJg0XAzFa9YZf5a9SvHXPi3VwXqS1TqFV5y2ky5UNy1R1bVQB0eoqRqLKFEOoDRIOx1G7OUkZ5GADFvNLaJcFnVumVCmtIrFLlkNHMuAFbzTXq9+fVPK9oSR0PIBBFbNLqXqRpfXNPL2ZoFWkb2m6DQqfUPpxKCKXTGpNAUlSDgJBWkEpUNwJOSOR1jL73tzSeha4v6f6D3tRhVKaT38pJyCgtDm9e5IIQFhW3Gh4cHkdRGnBs3R8Nh9agQPmf0EJD9D/7/AOq7Rjx2JZelHjLr+Ixw44SVNP69Pm7Y1UBBKSlIB+mOfhHm6X2CrUOhV66KjMzspXJqRSmQYeXJMSzLS9gS4n5XCFEjIO0cp88ZFoFWU5T+9fQoHbyqrT1PJKCk7SCeB1PBwM/WPfHVfVCZum3F0GbdeaqMul8MrW2UoQ+3kFKgD6pGcnGQeM8kxe1+CLenrJy+VG40PXw4eBVFkXLcGrOitm09VZfmEuXbblPptlE0+lJT3s6uXlJT5oHe5BxyAMZJINe7cvmhXNSKrWWLiqE/Sq7KTjlVSqXalEFtW5S3lEFbhWMb8eiRjHALPVyvXhRK3UqVWmFSFNlpOUYaSuYTsU8srGFGX9JO1QCgAffGtlGm5W1bGVpxXZWn2mLe6XLPB+YST3e3cXFHClFxoALUM5wFH2Rq8Q4mxCteqmUMlmqQ2/SDKWuLqSDmR5EAJBhWvGMOq23SRTzXOcXGdVriYJO6YJEgDkrrqFMkqJZ1bqlbkJepTFUSlpSqdMSja3Y5ltoBkFv1UnoMlOBjk5jQmn9OnrB0grdqSaZkI7d9qYkFNqHdSzJCSfWRkejygJWBnJA48YmfUevzWmGjdfq0tcU1+Xmln0s4bnN/cIS06phtIcaS35rAIJCUjJycHkxRxlmVmqpQp6kPuJlJuoMvNJbKkoUCtZ2gkAkZOMDxhUxZ11VfM09p7r0MR5DJST3S55iCBG0EJBJ8AYkPS5l+X0UrF9yr84/Va1OVZJSwjJQlJHdNn1d5HOeeM45HPkFxRCjrNy+f+yuuaqNLqL3eIkKyHQcFLe1IWE8cHI8iSPDHNFqnbpWjVJ5N3oiuVnSCWz0w0Qd7awdqkk7uhweOCPOJi6LGr1LaxqnWKtVS4xcYXKVJ5iWLqo4/3TzrZKsAbTgFRT6oyM+OI3H2mT+pknLT1TmX5t+5JSUpmoSrfpE4gFJKSncFJ3kZ3Z5wffFRn2bNqJhFGh5hL23cCRAHLtA6eLUiGl7hVNy2LZNQ3uNbAa8LbCjOTI5qB95VEbZa01TDm3bYa9UsBJRgnHjHYhCNdVdIQhBEhCEEXBUfufM/klfuManY7H5VH7nzP5JX7jGp2O0dEns3f6P3rHX/u+q8bqn9xXQhCLHrCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIkIQgiQhCCJCEIIv//Z" alt="PMAX" class="logo-img"></a>
    <span class="header-tag">Client Brief Form</span>
  </div>
</header>

<div class="hero">
  <div class="hero-inner">
    <div class="hero-eyebrow">Bắt đầu dự án của bạn</div>
    <h1>Chia sẻ thông tin<br>về chiến dịch của bạn</h1>
    <p>Chỉ mất khoảng 5–8 phút. Thông tin này giúp đội ngũ PMAX hiểu rõ mục tiêu và chuẩn bị đề xuất phù hợp nhất.</p>
  </div>
</div>

<div class="progress-wrap">
  <div class="progress-info">
    <span class="progress-label">Tiến độ điền form</span>
    <span class="progress-count" id="progressCount">0 / 5 bước</span>
  </div>
  <div class="progress-bar"><div class="progress-fill" id="progressFill"></div></div>
</div>

<div class="stepper" id="stepper">
  <button class="step-btn active" onclick="stepClick(0)"><span class="step-num">1</span> Người gửi brief</button>
  <button class="step-btn" onclick="stepClick(1)"><span class="step-num">2</span> Công ty & Thị trường</button>
  <button class="step-btn" onclick="stepClick(2)"><span class="step-num">3</span> Sản phẩm & Khách hàng</button>
  <button class="step-btn" onclick="stepClick(3)"><span class="step-num">4</span> KPI & Yêu cầu</button>
  <button class="step-btn" onclick="stepClick(4)"><span class="step-num">5</span> Ngân sách & Timeline</button>
  <button class="step-btn" onclick="stepClick(5)"><span class="step-num">6</span> Xem lại & Gửi</button>
</div>

<main class="main">

  <!-- STEP 1 -->
  <div class="section-card active" id="step-0">
    <div class="section-header">
      <div class="section-icon">👤</div>
      <div>
        <div class="section-label">Bước 1 / 6</div>
        <div class="section-title">Người gửi brief</div>
        <div class="section-desc">Thông tin để PMAX liên hệ lại với bạn.</div>
      </div>
    </div>
    <div class="section-body">
      <div class="field-row">
        <div class="field" id="f-company">
          <label>Tên công ty <span class="req">*</span></label>
          <input type="text" id="company" placeholder="VD: Unilever Việt Nam, Masan Consumer">
        </div>
        <div class="field" id="f-brand">
          <label>Thương hiệu / Sản phẩm <span class="req">*</span></label>
          <input type="text" id="brand" placeholder="VD: OMO, Chin-su, Kokomi">
        </div>
      </div>
      <div class="field-row">
        <div class="field" id="f-pic-name">
          <label>Họ tên người gửi brief <span class="req">*</span></label>
          <input type="text" id="picName" placeholder="VD: Nguyễn Thị Mai">
        </div>
        <div class="field" id="f-pic-title">
          <label>Chức vụ <span class="req">*</span></label>
          <input type="text" id="picTitle" placeholder="VD: Brand Manager">
        </div>
      </div>
      <div class="field">
        <label>Vai trò trong dự án <span class="req">*</span></label>
        <div class="radio-opts">
          <div class="radio-item" onclick="selectRadio(this,'picRole','dm')">
            <input type="radio" name="picRole" value="Decision Maker (người ra quyết định)">
            <span class="radio-dot"></span>
            <span class="radio-content"><span class="radio-label">Decision Maker</span><span class="radio-sub">Người ra quyết định cuối cùng</span></span>
          </div>
          <div class="radio-item" onclick="selectRadio(this,'picRole','lead')">
            <input type="radio" name="picRole" value="Project Lead (người quản lý dự án)">
            <span class="radio-dot"></span>
            <span class="radio-content"><span class="radio-label">Project Lead</span><span class="radio-sub">Người quản lý & điều phối dự án</span></span>
          </div>
          <div class="radio-item" onclick="selectRadio(this,'picRole','connector')">
            <input type="radio" name="picRole" value="Connector (người kết nối)">
            <span class="radio-dot"></span>
            <span class="radio-content"><span class="radio-label">Connector</span><span class="radio-sub">Người kết nối giữa các bên</span></span>
          </div>
          <div class="radio-item" onclick="selectRadio(this,'picRole','other')">
            <input type="radio" name="picRole" value="Khác">
            <span class="radio-dot"></span>
            <span class="radio-content"><span class="radio-label">Khác</span><span class="radio-sub">Vai trò khác trong tổ chức</span></span>
          </div>
        </div>
      </div>
      <div class="field-row">
        <div class="field" id="f-pic-email">
          <label>Email công việc <span class="req">*</span></label>
          <input type="email" id="picEmail" placeholder="ten@congty.com">
        </div>
        <div class="field" id="f-pic-phone">
          <label>Số điện thoại <span class="req">*</span></label>
          <input type="tel" id="picPhone" placeholder="0901 234 567">
        </div>
      </div>
      <div class="nav-row">
        <span></span>
        <button class="btn btn-primary" onclick="nextStep(0)">Tiếp theo →</button>
      </div>
    </div>
  </div>

  <!-- STEP 2 -->
  <div class="section-card" id="step-1">
    <div class="section-header">
      <div class="section-icon">🏢</div>
      <div>
        <div class="section-label">Bước 2 / 6</div>
        <div class="section-title">Công ty & Thị trường</div>
        <div class="section-desc">Bức tranh tổng quan về công ty và bối cảnh chiến dịch.</div>
      </div>
    </div>
    <div class="section-body">
      <div class="field" id="f-industry">
        <label>Lĩnh vực kinh doanh <span class="req">*</span></label>
        <select id="industry">
          <option value="">-- Chọn lĩnh vực --</option>
          <option>Ô tô / Xe máy</option>
          <option>Bất động sản</option>
          <option>Tài chính / Ngân hàng / Bảo hiểm</option>
          <option>Sức khỏe / Y tế / Dược phẩm</option>
          <option>Làm đẹp / Chăm sóc cá nhân</option>
          <option>Thực phẩm & Đồ uống (FMCG)</option>
          <option>Giáo dục</option>
          <option>Thương mại điện tử / Retail</option>
          <option>Công nghệ / SaaS</option>
          <option>Khác</option>
        </select>
      </div>
      <div class="field">
        <label>Kênh kỹ thuật số & kênh bán hàng đang có</label>
        <div class="hint">Paste link vào, ví dụ: Website, Facebook, TikTok, Shopee, Lazada…</div>
        <textarea id="channels" rows="3" placeholder="Website: https://&#10;Facebook: https://&#10;Shopee: https://&#10;Lazada: https://"></textarea>
      </div>
      <div class="field">
        <label>Bối cảnh & Thách thức hiện tại <span class="req">*</span></label>
        <div class="hint">Bối cảnh công ty hiện tại? Khó khăn, thách thức đang gặp phải là gì?</div>
        <textarea id="challenge" rows="3" placeholder="Mô tả tình hình hiện tại và lý do triển khai chiến dịch lần này…"></textarea>
      </div>
      <div class="field">
        <label>Đối thủ cạnh tranh chính</label>
        <input type="text" id="competitors" placeholder="VD: Brand A, Brand B…">
      </div>
      <div class="field">
        <label>Mục tiêu chiến dịch <span class="req">*</span></label>
        <div class="hint">Mục tiêu kinh doanh, mục tiêu truyền thông, và mục tiêu của chiến dịch này là gì?</div>
        <textarea id="goals" rows="3" placeholder="Mô tả mục tiêu cụ thể, kèm con số kỳ vọng nếu có…"></textarea>
      </div>
      <div class="field">
        <label>Chiến lược & tài nguyên marketing hiện có</label>
        <div class="hint">Đã có định hướng chiến lược chưa? Có KV, creative asset, tài liệu tham khảo sẵn không?</div>
        <textarea id="strategy" rows="2" placeholder="Mô tả chiến lược và tài nguyên hiện có…"></textarea>
      </div>
      <div class="field">
        <label>Công ty hiện đang tự vận hành marketing hay có đối tác hỗ trợ?</label>
        <div class="radio-opts">
          <div class="radio-item" onclick="selectRadio(this,'agencyType','inhouse')">
            <input type="radio" name="agencyType" value="inhouse">
            <span class="radio-dot"></span>
            <span class="radio-content"><span class="radio-label">Inhouse hoàn toàn</span><span class="radio-sub">Đội ngũ nội bộ tự thực hiện</span></span>
          </div>
          <div class="radio-item" onclick="selectRadio(this,'agencyType','agency')">
            <input type="radio" name="agencyType" value="agency">
            <span class="radio-dot"></span>
            <span class="radio-content"><span class="radio-label">Có agency hỗ trợ</span><span class="radio-sub">Đang hoặc từng làm với agency</span></span>
          </div>
          <div class="radio-item" onclick="selectRadio(this,'agencyType','hybrid')">
            <input type="radio" name="agencyType" value="hybrid">
            <span class="radio-dot"></span>
            <span class="radio-content"><span class="radio-label">Kết hợp cả hai</span><span class="radio-sub">Inhouse một phần, agency một phần</span></span>
          </div>
          <div class="radio-item" onclick="selectRadio(this,'agencyType','new')">
            <input type="radio" name="agencyType" value="new">
            <span class="radio-dot"></span>
            <span class="radio-content"><span class="radio-label">Chưa từng chạy marketing</span><span class="radio-sub">Đây là chiến dịch đầu tiên</span></span>
          </div>
        </div>
        <div id="agency-detail-wrap" style="display:none;margin-top:8px;">
          <input type="text" id="agencyDetail" placeholder="Tên agency đang / đã làm việc cùng">
        </div>
      </div>
      <div class="nav-row">
        <button class="btn btn-ghost" onclick="prevStep(1)">← Quay lại</button>
        <button class="btn btn-primary" onclick="nextStep(1)">Tiếp theo →</button>
      </div>
    </div>
  </div>

  <!-- STEP 3 -->
  <div class="section-card" id="step-2">
    <div class="section-header">
      <div class="section-icon">🛍️</div>
      <div>
        <div class="section-label">Bước 3 / 6</div>
        <div class="section-title">Sản phẩm & Khách hàng</div>
        <div class="section-desc">Thông tin về sản phẩm và đối tượng mục tiêu của chiến dịch.</div>
      </div>
    </div>
    <div class="section-body">
      <div class="field">
        <label>Thông tin sản phẩm / dịch vụ <span class="req">*</span></label>
        <div class="hint">Công ty đang cung cấp gì? Chiến lược sản phẩm ngắn hạn và dài hạn?</div>
        <textarea id="product" rows="3" placeholder="Mô tả sản phẩm/dịch vụ và định hướng phát triển…"></textarea>
      </div>
      <div class="field">
        <label>USP – Điểm khác biệt của sản phẩm</label>
        <div class="hint">Điều gì làm sản phẩm/dịch vụ của bạn nổi bật hơn đối thủ?</div>
        <textarea id="usp" rows="2" placeholder="Mô tả điểm khác biệt và lợi thế cạnh tranh…"></textarea>
      </div>
      <div class="field">
        <label>Giá sản phẩm / dịch vụ</label>
        <input type="text" id="price" placeholder="VD: 500.000 – 2.000.000 VND">
      </div>
      <div class="field">
        <label>Chân dung khách hàng mục tiêu <span class="req">*</span></label>
        <div class="hint">Độ tuổi, giới tính, địa lý, hành vi tiêu dùng, thu nhập…</div>
        <textarea id="audience" rows="3" placeholder="Mô tả chi tiết chân dung khách hàng mục tiêu…"></textarea>
      </div>
      <div class="nav-row">
        <button class="btn btn-ghost" onclick="prevStep(2)">← Quay lại</button>
        <button class="btn btn-primary" onclick="nextStep(2)">Tiếp theo →</button>
      </div>
    </div>
  </div>

  <!-- STEP 4 -->
  <div class="section-card" id="step-3">
    <div class="section-header">
      <div class="section-icon">🎯</div>
      <div>
        <div class="section-label">Bước 4 / 6</div>
        <div class="section-title">KPI & Yêu cầu dự án</div>
        <div class="section-desc">Các chỉ số mục tiêu và dịch vụ cần PMAX hỗ trợ.</div>
      </div>
    </div>
    <div class="section-body">
      <div class="field">
        <label>KPI muốn đạt được <span class="req">*</span></label>
        <div class="hint">Vui lòng nêu mức độ ưu tiên nếu có nhiều KPI</div>
        <textarea id="kpi" rows="3" placeholder="Nêu rõ chỉ số & mức mục tiêu cho từng KPI…"></textarea>
      </div>
      <div class="field">
        <label>Diễn giải chi tiết về KPI</label>
        <div class="hint">Cách đo lường, điều kiện tính là đạt, những điểm cần lưu ý</div>
        <textarea id="kpiDef" rows="2" placeholder="Định nghĩa cụ thể cho từng KPI…"></textarea>
      </div>
      <div class="field">
        <label>Hệ thống tracking đang dùng</label>
        <input type="text" id="tracking" placeholder="VD: Google Analytics, Meta Pixel, CRM…">
      </div>
      <div class="field">
        <label>Historical data – Dữ liệu chiến dịch đã triển khai</label>
        <div class="nda-badge">PMAX cam kết ký NDA bảo mật thông tin trước khi nhận data từ phía khách hàng</div>
        <div class="hint" style="margin-top:6px;">Kết quả các chiến dịch đã chạy, benchmark, chỉ số tham khảo… <a href="https://docs.google.com/document/d/1CJCNknEwbKK15S7fonSVbQE7Ah3yLnETqNBfjoqhOuU/edit?usp=sharing" target="_blank" style="color:var(--pmax-blue);font-weight:600;text-decoration:none;">Xem hướng dẫn điền data →</a></div>
        <textarea id="history" rows="3" placeholder="VD: Facebook Ads Q1/2025 - CPM 45k, CTR 1.2%, ROAS 3.5x&#10;Google Ads - CPC 8k, CVR 2.1%…"></textarea>
      </div>
      <div class="field">
        <label>Dịch vụ & Phạm vi công việc cần PMAX hỗ trợ <span class="req">*</span></label>
        <textarea id="services" rows="4" placeholder="Mô tả dịch vụ và yêu cầu cụ thể bạn cần. Ví dụ: Paid Social (Facebook, TikTok), Google Ads, Creative production, Landing page…"></textarea>
      </div>
      <div class="nav-row">
        <button class="btn btn-ghost" onclick="prevStep(3)">← Quay lại</button>
        <button class="btn btn-primary" onclick="nextStep(3)">Tiếp theo →</button>
      </div>
    </div>
  </div>

  <!-- STEP 5 -->
  <div class="section-card" id="step-4">
    <div class="section-header">
      <div class="section-icon">💰</div>
      <div>
        <div class="section-label">Bước 5 / 6</div>
        <div class="section-title">Ngân sách & Timeline</div>
        <div class="section-desc">Ngân sách, thời gian triển khai và thông tin pitching.</div>
      </div>
    </div>
    <div class="section-body">
      <div class="field" id="f-budget">
        <label>Ngân sách chiến dịch <span class="req">*</span></label>
        <div class="hint">Chọn mức phù hợp, sau đó điền ngân sách cụ thể của dự án lần này hoặc theo tháng</div>
        <div class="budget-tiers">
          <div class="tier-btn" onclick="selectTier(this,'lt100')"><div class="tier-value">&lt; 100 triệu</div><div class="tier-label">/ tháng</div></div>
          <div class="tier-btn" onclick="selectTier(this,'lt300')"><div class="tier-value">100 – &lt;300 triệu</div><div class="tier-label">/ tháng</div></div>
          <div class="tier-btn" onclick="selectTier(this,'gt300')"><div class="tier-value">&gt; 300 triệu</div><div class="tier-label">/ tháng</div></div>
        </div>
        <div id="budgetExactWrap" style="display:none;margin-top:2px;">
          <input type="text" id="budgetExact" placeholder="VD: 150 triệu VND/tháng hoặc 450 triệu VND cho cả dự án">
        </div>
      </div>
      <div class="field" id="f-vat">
        <label>Ngân sách trên đã bao gồm VAT & AF chưa? <span class="req">*</span></label>
        <div class="vat-opts">
          <button class="vat-btn" onclick="selectVat(this,'included')">Đã bao gồm VAT & AF</button>
          <button class="vat-btn" onclick="selectVat(this,'excluded')">Chưa bao gồm VAT & AF</button>
          <button class="vat-btn" onclick="selectVat(this,'unsure')">Chưa xác định</button>
        </div>
      </div>
      <div class="field" id="f-deadline">
        <label>Deadline nộp proposal / báo giá <span class="req">*</span></label>
        <input type="date" id="deadline">
      </div>
      <div class="field-row">
        <div class="field">
          <label>Ngày bắt đầu dự kiến <span class="req">*</span></label>
          <div class="hint">Ngày dự kiến khởi động triển khai dự án</div>
          <input type="date" id="startDate">
        </div>
        <div class="field" id="f-duration">
          <label>Thời gian triển khai dự án <span class="req">*</span></label>
          <div class="hint">Tổng thời lượng từ khi bắt đầu đến khi kết thúc dự án</div>
          <div class="duration-opts" style="margin-top:4px;">
            <button class="dur-btn" onclick="selectDur(this,'1m')">1 tháng</button>
            <button class="dur-btn" onclick="selectDur(this,'3m')">3 tháng</button>
            <button class="dur-btn" onclick="selectDur(this,'6m')">6 tháng</button>
            <button class="dur-btn" onclick="selectDur(this,'1y')">1 năm</button>
            <button class="dur-btn" onclick="selectDur(this,'custom')">Khác</button>
          </div>
          <input type="text" id="durationCustom" placeholder="VD: 2 tháng, 45 ngày…" style="margin-top:8px;display:none;">
        </div>
      </div>
      <div class="field">
        <label>Giai đoạn cao điểm / ghi chú timeline</label>
        <textarea id="timelineNote" rows="2" placeholder="Có giai đoạn tập trung cao điểm nào không? Tỉ trọng ngân sách từng giai đoạn nếu có…"></textarea>
      </div>
      <div class="field" id="f-pitching">
        <label>Dự án này có pitching không? <span class="req">*</span></label>
        <div class="radio-opts">
          <div class="radio-item" onclick="selectRadio(this,'pitchingYN','yes');togglePitching('yes')">
            <input type="radio" name="pitchingYN" value="yes">
            <span class="radio-dot"></span>
            <span class="radio-content"><span class="radio-label">Có pitching</span><span class="radio-sub">Nhiều agency tham gia đấu thầu</span></span>
          </div>
          <div class="radio-item" onclick="selectRadio(this,'pitchingYN','no');togglePitching('no')">
            <input type="radio" name="pitchingYN" value="no">
            <span class="radio-dot"></span>
            <span class="radio-content"><span class="radio-label">Không pitching</span><span class="radio-sub">Làm việc trực tiếp với PMAX</span></span>
          </div>
        </div>
      </div>
      <div id="pitching-detail-wrap" style="display:none;flex-direction:column;gap:14px;">
        <div class="field" id="f-pitchingAgencyCount">
          <label>Số lượng agency tham gia <span class="req">*</span></label>
          <input type="text" id="pitchingAgencyCount" placeholder="VD: 3 agencies">
        </div>
        <div class="field" id="f-pitchingTimeline">
          <label>Số vòng & timeline cột mốc từng vòng <span class="req">*</span></label>
          <div class="hint">Nêu rõ số vòng, deadline nộp và lịch thuyết trình từng vòng</div>
          <textarea id="pitchingTimeline" rows="4" placeholder="VD:&#10;2 vòng&#10;Vòng 1: Nộp proposal – 15/06&#10;Vòng 2: Thuyết trình – 22/06&#10;Thông báo kết quả – 25/06"></textarea>
        </div>
        <div class="field" id="f-criteria">
          <label>Tiêu chí đánh giá khi lựa chọn agency <span class="req">*</span></label>
          <textarea id="criteria" rows="2" placeholder="Sắp xếp theo mức độ ưu tiên từ cao xuống thấp…"></textarea>
        </div>
      </div>
      <div class="nav-row">
        <button class="btn btn-ghost" onclick="prevStep(4)">← Quay lại</button>
        <button class="btn btn-primary" onclick="nextStep(4)">Xem lại →</button>
      </div>
    </div>
  </div>

  <!-- STEP 6: Review -->
  <div class="section-card" id="step-5">
    <div class="section-header">
      <div class="section-icon">✅</div>
      <div>
        <div class="section-label">Bước 6 / 6</div>
        <div class="section-title">Xem lại thông tin</div>
        <div class="section-desc">Kiểm tra lại trước khi gửi. Click "Chỉnh sửa" ở từng mục để quay lại bổ sung.</div>
      </div>
    </div>
    <div class="section-body">
      <div id="summaryContent"></div>
      <div class="nav-row">
        <button class="btn btn-ghost" onclick="prevStep(5)">← Chỉnh sửa</button>
        <button class="btn btn-submit" onclick="submitForm()">🚀 Gửi Brief cho PMAX</button>
      </div>
    </div>
  </div>

  <!-- SUCCESS -->
  <div class="success-card" id="successCard">
    <div class="success-icon">🎉</div>
    <div class="success-title">Đã nhận được Brief!</div>
    <div class="success-sub">Cảm ơn bạn đã chia sẻ thông tin. Đội ngũ PMAX sẽ liên hệ với bạn trong vòng <strong>1 ngày làm việc</strong>.</div>
    <div class="success-detail" id="successDetail"></div>
  </div>

</main>

<footer class="site-footer">
  © 2025 PMAX Agency · <a href="https://pmax.vn" target="_blank">pmax.vn</a> · Thông tin được bảo mật và chỉ dùng nội bộ
</footer>

<script>
  let currentStep = 0;
  const totalSteps = 6;
  let budgetTier = '';
  let duration = '';
  let vatStatus = '';
  const doneSteps = new Set();

  function togglePitching(val) {
    const wrap = document.getElementById('pitching-detail-wrap');
    wrap.style.display = val === 'yes' ? 'flex' : 'none';
  }

  function stepClick(n) {
    if (n === currentStep) return;
    // allow navigation to any step for preview, but warn if going forward past unfinished
    goStep(n);
  }

  function goStep(n) {
    document.querySelectorAll('.section-card').forEach(c => c.classList.remove('active'));
    document.getElementById('step-' + n).classList.add('active');
    currentStep = n;
    updateProgress();
    updateStepper();
    if (n === 5) buildSummary();
    window.scrollTo({ top: 0, behavior: 'smooth' });
  }
  function nextStep(from) { if (!validateStep(from)) return; doneSteps.add(from); goStep(from + 1); }
  function prevStep(from) { goStep(from - 1); }

  function updateProgress() {
    const pct = (doneSteps.size / (totalSteps - 1)) * 100;
    document.getElementById('progressFill').style.width = Math.min(pct, 100) + '%';
    document.getElementById('progressCount').textContent = doneSteps.size + ' / ' + (totalSteps - 1) + ' bước';
  }
  function updateStepper() {
    document.querySelectorAll('.step-btn').forEach((btn, i) => {
      btn.classList.remove('active', 'done', 'preview');
      if (i === currentStep) btn.classList.add('active');
      else if (doneSteps.has(i)) btn.classList.add('done');
      else btn.classList.add('preview');
    });
  }

  function clearErrors() {
    document.querySelectorAll('.field.error').forEach(f => {
      f.classList.remove('error');
      f.querySelectorAll('.field-err').forEach(e => e.remove());
    });
  }
  function showErr(wrap, msg) {
    wrap.querySelectorAll('.field-err').forEach(e => e.remove());
    const e = document.createElement('span'); e.className = 'field-err'; e.textContent = msg;
    wrap.appendChild(e);
  }
  function markError(el, msg) {
    const wrap = el.closest('.field') || el.parentElement;
    wrap.classList.add('error'); showErr(wrap, msg);
  }
  function errById(inputId, wrapId, msg) {
    const el = document.getElementById(inputId);
    const wrap = wrapId ? document.getElementById(wrapId) : el?.closest('.field');
    if (!el || !el.value.trim()) { if (wrap) { wrap.classList.add('error'); showErr(wrap, msg); } return false; }
    return true;
  }

  function validateStep(step) {
    let ok = true; clearErrors();

    if (step === 0) {
      if (!errById('company','f-company','Vui lòng nhập tên công ty')) ok = false;
      if (!errById('brand','f-brand','Vui lòng nhập tên thương hiệu')) ok = false;
      if (!errById('picName','f-pic-name','Vui lòng nhập họ tên người gửi brief')) ok = false;
      if (!errById('picTitle','f-pic-title','Vui lòng nhập chức vụ')) ok = false;
      if (!errById('picEmail','f-pic-email','Vui lòng nhập email')) ok = false;
      const emailEl = document.getElementById('picEmail');
      if (emailEl.value && !emailEl.value.includes('@')) {
        const w = document.getElementById('f-pic-email');
        if (!w.classList.contains('error')) { w.classList.add('error'); showErr(w,'Email không hợp lệ'); ok = false; }
      }
      if (!errById('picPhone','f-pic-phone','Vui lòng nhập số điện thoại')) ok = false;
      if (!document.querySelector('input[name="picRole"]:checked')) {
        const w = document.querySelector('input[name="picRole"]').closest('.field');
        w.classList.add('error'); showErr(w,'Vui lòng chọn vai trò trong dự án'); ok = false;
      }
    }

    if (step === 1) {
      if (!errById('industry','f-industry','Vui lòng chọn lĩnh vực kinh doanh')) ok = false;
      [['challenge','Vui lòng mô tả bối cảnh & thách thức'],['goals','Vui lòng mô tả mục tiêu chiến dịch']].forEach(([id,msg]) => {
        const el = document.getElementById(id);
        if (!el.value.trim()) { markError(el,msg); ok = false; }
      });
    }

    if (step === 2) {
      [['product','Vui lòng mô tả sản phẩm / dịch vụ'],['audience','Vui lòng mô tả khách hàng mục tiêu']].forEach(([id,msg]) => {
        const el = document.getElementById(id);
        if (!el.value.trim()) { markError(el,msg); ok = false; }
      });
    }

    if (step === 3) {
      [['kpi','Vui lòng điền KPI muốn đạt được'],['services','Vui lòng mô tả dịch vụ và yêu cầu cụ thể']].forEach(([id,msg]) => {
        const el = document.getElementById(id);
        if (!el.value.trim()) { markError(el,msg); ok = false; }
      });
    }

    if (step === 4) {
      if (!budgetTier) {
        const w = document.querySelector('.budget-tiers').closest('.field');
        w.classList.add('error'); showErr(w,'Vui lòng chọn mức ngân sách'); ok = false;
      }
      if (!errById('budgetExact',null,'Vui lòng điền ngân sách cụ thể')) ok = false;
      if (!vatStatus) {
        const w = document.getElementById('f-vat');
        w.classList.add('error'); showErr(w,'Vui lòng chọn trạng thái VAT & AF'); ok = false;
      }
      if (!errById('deadline','f-deadline','Vui lòng chọn deadline nộp proposal')) ok = false;
      if (!errById('startDate',null,'Vui lòng chọn ngày bắt đầu')) ok = false;
      if (!duration) {
        const w = document.getElementById('f-duration');
        w.classList.add('error'); showErr(w,'Vui lòng chọn thời gian triển khai dự án'); ok = false;
      }
      const pitchEl = document.querySelector('input[name="pitchingYN"]:checked');
      if (!pitchEl) {
        const w = document.getElementById('f-pitching');
        w.classList.add('error'); showErr(w,'Vui lòng chọn có pitching hay không'); ok = false;
      } else if (pitchEl.value === 'yes') {
        if (!errById('pitchingAgencyCount','f-pitchingAgencyCount','Vui lòng điền số lượng agency tham gia')) ok = false;
        const tlEl = document.getElementById('pitchingTimeline');
        if (!tlEl.value.trim()) { markError(tlEl,'Vui lòng điền số vòng & timeline cột mốc'); ok = false; }
        const crEl = document.getElementById('criteria');
        if (!crEl.value.trim()) { markError(crEl,'Vui lòng điền tiêu chí đánh giá'); ok = false; }
      }
    }

    if (!ok) {
      const firstErr = document.querySelector('#step-' + step + ' .error');
      if (firstErr) firstErr.scrollIntoView({ behavior:'smooth', block:'center' });
    }
    return ok;
  }

  function selectRadio(el, name, val) {
    document.querySelectorAll(`.radio-item input[name="${name}"]`).forEach(r => {
      r.closest('.radio-item').classList.remove('selected'); r.checked = false;
    });
    el.classList.add('selected');
    const radio = el.querySelector('input[type="radio"]');
    if (radio) radio.checked = true;
    if (name === 'agencyType') {
      document.getElementById('agency-detail-wrap').style.display = (val === 'agency' || val === 'hybrid') ? 'block' : 'none';
    }
  }
  function selectTier(el, val) {
    document.querySelectorAll('.tier-btn').forEach(b => b.classList.remove('selected'));
    el.classList.add('selected'); budgetTier = val;
    document.getElementById('budgetExactWrap').style.display = 'block';
    document.getElementById('budgetExact').focus();
  }
  function selectDur(el, val) {
    document.querySelectorAll('.dur-btn').forEach(b => b.classList.remove('selected'));
    el.classList.add('selected'); duration = val;
    document.getElementById('durationCustom').style.display = val === 'custom' ? 'block' : 'none';
  }
  function selectVat(el, val) {
    document.querySelectorAll('.vat-btn').forEach(b => b.classList.remove('selected'));
    el.classList.add('selected'); vatStatus = val;
  }

  function buildSummary() {
    const tierMap = { lt100:'< 100 triệu/tháng', lt300:'100 - <300 triệu/tháng', gt300:'> 300 triệu/tháng' };
    const durMap  = { '1m':'1 tháng','3m':'3 tháng','6m':'6 tháng','1y':'1 năm','custom':v('durationCustom')||'Khác' };
    const vatMap  = { included:'Đã bao gồm VAT & AF', excluded:'Chưa bao gồm VAT & AF', unsure:'Chưa xác định' };
    const agencyMap = { inhouse:'Inhouse hoàn toàn', agency:'Có agency hỗ trợ', hybrid:'Kết hợp cả hai', new:'Chưa từng chạy marketing' };
    const roleEl   = document.querySelector('input[name="picRole"]:checked');
    const agencyEl = document.querySelector('input[name="agencyType"]:checked');
    const pitchEl  = document.querySelector('input[name="pitchingYN"]:checked');

    const row = (label, val) => {
      const display = val ? val : '<span class="summary-empty">-</span>';
      return `<div class="summary-row"><span class="summary-key">${label}</span><span class="summary-val">${display}</span></div>`;
    };
    const section = (title, stepIdx, rows) => `
      <div class="summary-section">
        <h3>${title}<button class="btn-edit-section" onclick="goStep(${stepIdx})">✏️ Chỉnh sửa</button></h3>
        ${rows}
      </div>`;

    document.getElementById('summaryContent').innerHTML =
      section('👤 Người gửi brief', 0,
        row('Công ty', v('company')) + row('Thương hiệu', v('brand')) +
        row('Họ tên', [v('picName'),v('picTitle')].filter(Boolean).join(' - ')) +
        row('Vai trò', roleEl ? roleEl.value : '') +
        row('Email', v('picEmail')) + row('Số điện thoại', v('picPhone'))
      ) +
      section('🏢 Công ty & Thị trường', 1,
        row('Lĩnh vực', v('industry')) + row('Kênh digital & bán hàng', v('channels')) +
        row('Bối cảnh & Thách thức', v('challenge')) + row('Đối thủ', v('competitors')) +
        row('Mục tiêu chiến dịch', v('goals')) + row('Chiến lược & tài nguyên', v('strategy')) +
        row('Hình thức vận hành', agencyEl ? (agencyMap[agencyEl.value]+(v('agencyDetail')?' - '+v('agencyDetail'):'')) : '')
      ) +
      section('🛍️ Sản phẩm & Khách hàng', 2,
        row('Sản phẩm / dịch vụ', v('product')) + row('USP', v('usp')) +
        row('Giá', v('price')) + row('Khách hàng mục tiêu', v('audience'))
      ) +
      section('🎯 KPI & Yêu cầu', 3,
        row('KPI', v('kpi')) + row('Định nghĩa KPI', v('kpiDef')) +
        row('Tracking system', v('tracking')) + row('Historical data', v('history')) +
        row('Dịch vụ cần PMAX', v('services'))
      ) +
      section('💰 Ngân sách & Timeline', 4,
        row('Ngân sách', (tierMap[budgetTier]||'')+(v('budgetExact')?' · '+v('budgetExact'):'')) +
        row('VAT & AF', vatMap[vatStatus]||'') +
        row('Deadline proposal', v('deadline')) +
        row('Bắt đầu', v('startDate')) + row('Thời lượng', durMap[duration]||duration) +
        row('Ghi chú timeline', v('timelineNote')) +
        row('Pitching', pitchEl ? (pitchEl.value==='yes' ? 'Có pitching' : 'Không pitching') : '') +
        row('Số agency', v('pitchingAgencyCount')) + row('Số vòng', v('pitchingRounds')) +
        row('Timeline pitching', v('pitchingTimeline')) + row('Tiêu chí đánh giá', v('criteria'))
      );
  }

  function v(id) { const el = document.getElementById(id); return el ? (el.value||'') : ''; }

  async function submitForm() {
    const btn = document.querySelector('.btn-submit');
    btn.disabled = true; btn.textContent = '⏳ Đang gửi...';
    const payload = collectPayload();
    const SCRIPT_URL = 'PASTE_YOUR_APPS_SCRIPT_URL_HERE';
    try {
      if (SCRIPT_URL !== 'PASTE_YOUR_APPS_SCRIPT_URL_HERE') {
        await fetch(SCRIPT_URL, { method:'POST', mode:'no-cors', headers:{'Content-Type':'application/json'}, body:JSON.stringify(payload) });
      }
    } catch(err) { console.error('Submit error:', err); }
    showSuccess(payload);
  }

  function showSuccess(p) {
    document.querySelectorAll('.section-card').forEach(c => { c.style.display='none'; c.classList.remove('active'); });
    document.getElementById('stepper').style.display = 'none';
    document.querySelector('.progress-wrap').style.display = 'none';
    document.getElementById('successCard').classList.add('show');
    document.getElementById('successDetail').innerHTML =
      `<strong>Công ty:</strong> ${p.company} (${p.brand})<br>
       <strong>Người gửi:</strong> ${p.pic.name} · ${p.pic.email}<br>
       <strong>Ngân sách:</strong> ${p.budget.tier||'-'} · ${p.budget.exact}<br>
       <strong>Deadline proposal:</strong> ${p.deadline||'-'}<br>
       <strong>Bắt đầu dự kiến:</strong> ${p.startDate||'-'}`;
    window.scrollTo({ top:0, behavior:'smooth' });
  }

  function collectPayload() {
    const tierMap = { lt100:'< 100 triệu/tháng', lt300:'100 - <300 triệu/tháng', gt300:'> 300 triệu/tháng' };
    const durMap  = { '1m':'1 tháng','3m':'3 tháng','6m':'6 tháng','1y':'1 năm','custom':v('durationCustom')||'Khác' };
    const vatMap  = { included:'Đã bao gồm VAT & AF', excluded:'Chưa bao gồm VAT & AF', unsure:'Chưa xác định' };
    const agencyMap = { inhouse:'Inhouse hoàn toàn', agency:'Có agency hỗ trợ', hybrid:'Kết hợp cả hai', new:'Chưa từng chạy marketing' };
    const roleEl   = document.querySelector('input[name="picRole"]:checked');
    const agencyEl = document.querySelector('input[name="agencyType"]:checked');
    const pitchEl  = document.querySelector('input[name="pitchingYN"]:checked');
    return {
      timestamp: new Date().toISOString(),
      company: v('company'), brand: v('brand'), deadline: v('deadline'),
      pic: { name:v('picName'), title:v('picTitle'), role:roleEl?roleEl.value:'', email:v('picEmail'), phone:v('picPhone') },
      industry: v('industry'), channels: v('channels'),
      challenge: v('challenge'), competitors: v('competitors'), goals: v('goals'), strategy: v('strategy'),
      agencyType: agencyEl?agencyEl.value:'', agencyTypeLabel: agencyEl?(agencyMap[agencyEl.value]||''):'', agencyDetail: v('agencyDetail'),
      product: v('product'), usp: v('usp'), price: v('price'), audience: v('audience'),
      kpi: v('kpi'), kpiDef: v('kpiDef'), tracking: v('tracking'), history: v('history'), services: v('services'),
      budget: { tier:tierMap[budgetTier]||'', exact:v('budgetExact') },
      vatStatus: vatMap[vatStatus]||'',
      startDate: v('startDate'), duration, durationLabel: durMap[duration]||duration, timelineNote: v('timelineNote'),
      pitching: pitchEl?pitchEl.value:'',
      pitchingAgencyCount: v('pitchingAgencyCount'), pitchingRounds: v('pitchingRounds'),
      pitchingTimeline: v('pitchingTimeline'), criteria: v('criteria'),
    };
  }
</script>
</body>
</html>

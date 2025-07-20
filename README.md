# javvy-v2.css
/*
  FICHIER: assets/product-javvy-v2.css
  EMPLACEMENT: /assets/product-javvy-v2.css
  
  Style produit Javvy corrigé avec :
  - Layout responsive adaptatif
  - Bundle selector fonctionnel
  - Gallery images/vidéos
  - Interface vintage Harley
*/

/* === 🎯 CONTAINER PRINCIPAL === */
.harley-product-container {
  padding: 40px 0;
  background: linear-gradient(135deg, #fafafa 0%, #f5f5f5 100%);
  min-height: 100vh;
}

.container {
  max-width: 1400px;
  margin: 0 auto;
  padding: 0 20px;
}

.product-layout {
  display: grid;
  grid-template-columns: 1fr 320px;
  gap: 60px;
  align-items: start;
  position: relative;
  z-index: 10;
}

/* === 🎯 SECTION PRODUIT PRINCIPALE === */
.main-product {
  display: flex;
  flex-direction: column;
  gap: 40px;
}

/* === 🎯 GALLERY LAYOUT JAVVY-STYLE === */
.product-gallery {
  display: flex;
  flex-direction: column;
  gap: 20px;
}

.gallery-layout {
  display: grid;
  grid-template-columns: 1fr 140px;
  gap: 20px;
  align-items: start;
}

.main-image-container {
  width: 100%;
  position: relative;
  overflow: hidden;
  border-radius: 12px;
  box-shadow: 0 8px 30px rgba(0,0,0,0.12);
}

.product-image {
  width: 100%;
  max-width: 600px;
  height: auto;
  border-radius: 12px;
  transition: all 0.3s ease;
  display: block;
}

.product-image:hover {
  transform: scale(1.02);
}

/* Video styling */
.main-image-container video {
  width: 100%;
  max-width: 600px;
  height: auto;
  border-radius: 12px;
}

/* === 🎯 MINIATURES DROITE === */
.thumbnail-sidebar {
  display: flex;
  flex-direction: column;
  gap: 15px;
}

.thumbnail-right {
  width: 120px;
  height: 120px;
  border-radius: 8px;
  cursor: pointer;
  border: 2px solid transparent;
  transition: all 0.3s ease;
  object-fit: cover;
}

.thumbnail-right:hover,
.thumbnail-right.active {
  border-color: #FF8E20;
  box-shadow: 0 0 12px rgba(255, 142, 32, 0.5);
  transform: scale(1.05);
}

/* === 🎯 VIDEOS THUMBNAILS === */
.video-thumbnail-small {
  width: 120px;
  height: 120px;
  background: linear-gradient(135deg, #FF8E20, #D2691E);
  border-radius: 8px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  color: white;
  font-weight: 600;
  transition: all 0.3s ease;
  border: 2px solid transparent;
}

.video-thumbnail-small:hover,
.video-thumbnail-small.active {
  border-color: #8B4513;
  transform: scale(1.05);
  box-shadow: 0 0 12px rgba(139, 69, 19, 0.5);
}

.play-icon-small {
  font-size: 2rem;
  margin-bottom: 5px;
}

.video-label {
  font-size: 0.7rem;
  text-transform: uppercase;
}

/* === 🎯 IMAGES BOTTOM === */
.bottom-thumbnails {
  display: flex;
  gap: 15px;
  justify-content: flex-start;
  overflow-x: auto;
  padding-bottom: 10px;
}

.thumbnail-bottom {
  width: 350px;
  height: 200px;
  border-radius: 8px;
  cursor: pointer;
  border: 2px solid transparent;
  transition: all 0.3s ease;
  object-fit: cover;
  flex-shrink: 0;
}

.thumbnail-bottom:hover,
.thumbnail-bottom.active {
  border-color: #FF8E20;
  box-shadow: 0 0 12px rgba(255, 142, 32, 0.3);
  transform: scale(1.02);
}

.video-thumbnail-bottom {
  width: 350px;
  height: 200px;
  background: linear-gradient(135deg, #FF8E20, #D2691E);
  border-radius: 8px;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  color: white;
  font-weight: 600;
  transition: all 0.3s ease;
  border: 2px solid transparent;
  flex-shrink: 0;
}

.video-thumbnail-bottom:hover,
.video-thumbnail-bottom.active {
  border-color: #8B4513;
  transform: scale(1.02);
}

.play-icon-large {
  font-size: 4rem;
  margin-bottom: 10px;
}

.video-text {
  font-size: 1rem;
  text-transform: uppercase;
}

/* === 🎯 PRODUCT INFO === */
.product-info {
  display: flex;
  flex-direction: column;
  gap: 25px;
}

.product-rating {
  font-size: 1rem;
  color: #666;
  margin: 0;
}

.product-badges {
  display: flex;
  gap: 12px;
  flex-wrap: wrap;
}

.badge {
  background: linear-gradient(135deg, #F5DEB3, #DEB887);
  border: 1px solid #8B4513;
  color: #8B4513;
  font-weight: 600;
  text-shadow: 1px 1px 1px rgba(255,255,255,0.5);
  padding: 6px 14px;
  border-radius: 20px;
  font-size: 0.85rem;
  text-transform: uppercase;
  letter-spacing: 0.5px;
}

.product-title {
  font-size: 2.4rem;
  font-weight: 700;
  color: #8B4513;
  line-height: 1.2;
  margin: 0;
  text-shadow: 2px 2px 4px rgba(245, 222, 179, 0.5);
}

.product-description {
  font-size: 1.1rem;
  color: #666;
  line-height: 1.6;
  margin: 0;
}

/* === 🎯 BUILD BUNDLE SYSTÈME === */
.build-bundle h3 {
  font-size: 1.2rem;
  color: #8B4513;
  font-weight: 600;
  margin: 0 0 20px 0;
  text-shadow: 1px 1px 2px rgba(245, 222, 179, 0.5);
}

.bundle-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(120px, 1fr));
  gap: 15px;
  margin-bottom: 20px;
}

.bundle-item {
  background: linear-gradient(135deg, #FFF8DC, #F5DEB3);
  border: 2px solid #DEB887;
  border-radius: 8px;
  padding: 18px 12px;
  text-align: center;
  cursor: pointer;
  transition: all 0.3s ease;
  position: relative;
  min-height: 80px;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.bundle-item:hover {
  border-color: #FF8E20;
  transform: translateY(-2px);
  box-shadow: 0 4px 15px rgba(255, 142, 32, 0.3);
}

.bundle-item.selected {
  border-color: #FF8E20;
  background: linear-gradient(135deg, #FFF8DC, #F5DEB3);
  transform: translateY(-2px);
  box-shadow: 0 4px 15px rgba(255, 142, 32, 0.4);
}

.bundle-label {
  font-weight: 600;
  color: #8B4513;
  margin-bottom: 5px;
  font-size: 0.9rem;
  text-shadow: 1px 1px 1px rgba(255,255,255,0.5);
}

.bundle-price {
  font-size: 0.85rem;
  color: #8B4513;
  font-weight: 500;
}

.best-deal-badge {
  position: absolute;
  top: -8px;
  right: -5px;
  background: linear-gradient(135deg, #FF8E20, #D2691E);
  color: white;
  font-size: 0.65rem;
  padding: 3px 6px;
  border-radius: 3px;
  font-weight: 700;
  text-shadow: 1px 1px 2px rgba(0,0,0,0.3);
  border: 1px solid #8B4513;
  text-transform: uppercase;
  letter-spacing: 0.5px;
}

/* === 🎯 SUBSCRIBE SECTION === */
.subscribe-section {
  background: linear-gradient(135deg, #FFF8DC, #F5DEB3);
  border: 2px solid #DEB887;
  border-radius: 8px;
  padding: 20px;
  box-shadow: inset 0 2px 4px rgba(139, 69, 19, 0.1);
}

.subscribe-section h3 {
  color: #8B4513;
  margin: 0 0 12px 0;
  font-size: 1.1rem;
  text-shadow: 1px 1px 2px rgba(245, 222, 179, 0.5);
}

.subscribe-benefits {
  display: flex;
  flex-direction: column;
  gap: 8px;
}

.benefit-row {
  display: flex;
  align-items: center;
  gap: 8px;
  font-size: 0.9rem;
  color: #666;
}

.check {
  color: #FF8E20;
  font-weight: bold;
  font-size: 1rem;
}

/* === 🎯 PRICING SECTION === */
.pricing-section {
  border-top: 2px solid #DEB887;
  padding-top: 25px;
}

.current-selection {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
  padding: 15px;
  background: linear-gradient(135deg, #FFF8DC, #F5DEB3);
  border: 1px solid #DEB887;
  border-radius: 8px;
}

.qty-display,
.total-price {
  font-weight: 700;
  color: #8B4513;
  text-shadow: 1px 1px 1px rgba(255,255,255,0.5);
}

.main-add-to-cart {
  width: 100%;
  background: linear-gradient(135deg, #FF8E20, #D2691E);
  border: 2px solid #8B4513;
  color: white;
  padding: 18px 32px;
  font-size: 1.1rem;
  font-weight: 600;
  border-radius: 8px;
  cursor: pointer;
  transition: all 0.3s ease;
  text-shadow: 1px 1px 2px rgba(0,0,0,0.3);
  box-shadow: 0 4px 15px rgba(255, 142, 32, 0.4);
  text-transform: uppercase;
  letter-spacing: 1px;
}

.main-add-to-cart:hover {
  background: linear-gradient(135deg, #D2691E, #FF8E20);
  transform: translateY(-2px);
  box-shadow: 0 6px 20px rgba(255, 142, 32, 0.5);
}

.main-add-to-cart:disabled {
  background: #cccccc;
  border-color: #999999;
  cursor: not-allowed;
  transform: none;
  box-shadow: none;
}

.main-add-to-cart:disabled:hover {
  background: #cccccc;
  transform: none;
  box-shadow: none;
}

/* === 📱 RESPONSIVE === */
@media (max-width: 1024px) {
  .product-layout {
    grid-template-columns: 1fr;
    gap: 40px;
  }
  
  .bundle-grid {
    grid-template-columns: repeat(2, 1fr);
  }
  
  .gallery-layout {
    grid-template-columns: 1fr;
    gap: 20px;
  }
  
  .thumbnail-sidebar {
    flex-direction: row;
    gap: 10px;
    overflow-x: auto;
    padding-bottom: 10px;
  }
  
  .thumbnail-right {
    min-width: 80px;
    height: 80px;
  }
  
  .video-thumbnail-small {
    min-width: 80px;
    height: 80px;
  }
  
  .play-icon-small {
    font-size: 1.5rem;
  }
  
  .video-label {
    font-size: 0.6rem;
  }
}

@media (max-width: 768px) {
  .container {
    padding: 0 15px;
  }
  
  .product-title {
    font-size: 2rem;
  }
  
  .bundle-grid {
    grid-template-columns: 1fr;
  }
  
  .current-selection {
    flex-direction: column;
    gap: 10px;
    text-align: center;
  }
  
  .bottom-thumbnails {
    flex-direction: column;
    align-items: center;
  }
  
  .thumbnail-bottom,
  .video-thumbnail-bottom {
    width: 100%;
    max-width: 300px;
  }
  
  .main-add-to-cart {
    font-size: 1rem;
    padding: 15px 25px;
  }
}

@media (max-width: 480px) {
  .harley-product-container {
    padding: 20px 0;
  }
  
  .container {
    padding: 0 10px;
  }
  
  .main-product {
    gap: 30px;
  }
  
  .product-title {
    font-size: 1.8rem;
  }
  
  .product-badges {
    justify-content: center;
  }
  
  .badge {
    font-size: 0.75rem;
    padding: 4px 10px;
  }
  
  .bundle-item {
    padding: 12px 8px;
    min-height: 70px;
  }
  
  .bundle-label {
    font-size: 0.8rem;
  }
  
  .bundle-price {
    font-size: 0.75rem;
  }
  
  .best-deal-badge {
    font-size: 0.6rem;
    padding: 2px 4px;
  }
}

/* === 🎯 LOADING STATES === */
.main-add-to-cart.loading {
  opacity: 0.7;
  cursor: not-allowed;
  pointer-events: none;
}

.main-add-to-cart.loading::after {
  content: " ...";
  animation: loading-dots 1.5s infinite;
}

@keyframes loading-dots {
  0%, 20% { content: " "; }
  40% { content: " ."; }
  60% { content: " .."; }
  80%, 100% { content: " ..."; }
}

/* === 🎯 SUCCESS STATES === */
.main-add-to-cart.success {
  background: linear-gradient(135deg, #27ae60, #2ecc71);
  border-color: #1e8449;
}

.main-add-to-cart.success::after {
  content: " ✓";
}

/* === 🎯 FORM ELEMENTS === */
.add-to-cart-form {
  display: block;
  margin: 0;
}

.add-to-cart-form input[type="hidden"] {
  display: none;
}

/* === 🎯 ACCESSIBILITY === */
.bundle-item:focus,
.thumbnail-right:focus,
.thumbnail-bottom:focus,
.video-thumbnail-small:focus,
.video-thumbnail-bottom:focus {
  outline: 2px solid #FF8E20;
  outline-offset: 2px;
}

.main-add-to-cart:focus {
  outline: 2px solid #8B4513;
  outline-offset: 2px;
}

/* === 🎯 ANIMATIONS === */
@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.product-layout {
  animation: fadeIn 0.6s ease-out;
}

.bundle-item {
  animation: fadeIn 0.8s ease-out;
}

.bundle-item:nth-child(1) { animation-delay: 0.1s; }
.bundle-item:nth-child(2) { animation-delay: 0.2s; }
.bundle-item:nth-child(3) { animation-delay: 0.3s; }
.bundle-item:nth-child(4) { animation-delay: 0.4s; }
.bundle-item:nth-child(5) { animation-delay: 0.5s; }

/* === 🎯 PRINT STYLES === */
@media print {
  .harley-product-container {
    background: white;
  }
  
  .product-layout {
    grid-template-columns: 1fr;
    gap: 20px;
  }
  
  .flavors-sidebar,
  .main-add-to-cart,
  .subscribe-section {
    display: none;
  }
}

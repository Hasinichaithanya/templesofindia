<!-- javascript code -->
<script>
	export function closeItems(id, id2, id3) {
		let element = document.getElementById(id);
		let angleUpIcon = document.getElementById(id2);
		let angleDownIcon = document.getElementById(id3);
		if (element.classList.contains('hide-content')) {
			element.classList.remove('hide-content');
			angleDownIcon.classList.remove('hide-content');
			angleUpIcon.classList.add('hide-content');
		} else {
			element.classList.add('hide-content');
			angleDownIcon.classList.add('hide-content');
			angleUpIcon.classList.remove('hide-content');
		}
	}
	export function displaybutton() {
		let btn = document.getElementById('submitBtn');
		btn.classList.add('display-submit-btn');
		btn.classList.remove('submit-btn');
	}
</script>

<div class="main-container">
	<!-- navbar for desktop view -->
	<nav class="navbar">
		<a href="https://templesofindia.org/" class="logo">
			<img
				src="https://templesofindia.org/assets/images/tofi_logo/tofi-logo_navbar.png"
				alt="logo"
			/><span class="nav-temple-name">Temples of India</span>
		</a>
		<ul>
			<a href="https://templesofindia.org/">Home</a>
			<a
				href="https://templesofindia.org/temple-view/sri-ranganathar-temple-tamil-nadu-tamil-nadu-227bgo"
				>Search</a
			>
			<a href="https://templesofindia.org/nearbyTemples">Nearby Temples</a>
			<a href="https://templesofindia.org/addTemples">
				<img
					src="https://th.bing.com/th/id/OIP.1XquM5bWcbc4CRppG9E7EQHaHa?w=177&h=180&c=7&r=0&o=5&dpr=1.5&pid=1.7"
					alt=""
					class="add-temples"
				/>Add Temples
			</a>
			<a href="https://templesofindia.org/aboutUs">About Us</a>
			<a href="">Login</a>
		</ul>
	</nav>
	<!-- navbar for mobile view -->

	<div class="mobile-nav">
		<button
			class="cross-btn"
			type="button"
			data-bs-toggle="offcanvas"
			data-bs-target="#offcanvasWithBothOptions"
			aria-controls="offcanvasWithBothOptions"><i class="fa-solid fa-bars"></i></button
		>
		<b
			><img
				src="https://templesofindia.org/assets/images/tofi_logo/tofi-logo_navbar.png"
				alt="logo"
			/>TEMPLES OF INDIA</b
		> <i class="fa-solid fa-magnifying-glass"></i>
	</div>
	<!-- sidebar for mobile view -->

	<div
		class="offcanvas offcanvas-start sidebar"
		data-bs-scroll="true"
		tabindex="-1"
		id="offcanvasWithBothOptions"
		aria-labelledby="offcanvasWithBothOptionsLabel"
	>
		<div class="offcanvas-header off-canvas">
			<button
				type="button"
				id="closeBtn"
				class="btn-close"
				data-bs-dismiss="offcanvas"
				aria-label="Close"
			></button>
		</div>
		<div class="offcanvas-body">
			<div class="profile-details">
				<img
					src="https://templesofindia.org/assets/images/Golden-Temple.jpg"
					alt=""
					class="profile-img"
				/>
				<div>
					<p>Username</p>
					<p>View Profile</p>
				</div>
			</div>
			<div class="sidebar-item">
				<i class="fa-solid fa-house"></i> Home
			</div>
			<hr />
			<div class="sidebar-item"><i class="fa-solid fa-key"></i>Login</div>
			<hr />
			<div class="sidebar-item"><i class="fa-solid fa-gopuram"></i>Nearby Temples</div>
			<hr />
			<div class="sidebar-item">
				<img
					src="https://th.bing.com/th/id/OIP.1XquM5bWcbc4CRppG9E7EQHaHa?w=177&h=180&c=7&r=0&o=5&dpr=1.5&pid=1.7"
					alt=""
					class="add-temples"
				/>Add Temples
			</div>
			<hr />
			<div class="sidebar-item"><i class="fa-solid fa-circle-info"></i>About Us</div>
			<hr />
			<div class="sidebar-item"><i class="fa-solid fa-star"></i> Download App</div>
			<hr />
		</div>
	</div>

	<!-- image container -->
	<div>
		<img
			src="https://templesofindia.org/assets/compressed/tofi-banner.jpg"
			alt="toi"
			class="temple-image"
		/>
		<div class="icons desktop-location-view">
			<div class="two-icons-desktop">
				<img
					src="https://templesofindia.org/assets/icons/custom_visited.svg"
					alt=""
					class="visted-img"
				/>
				<span>Visited</span>
			</div>
			<div class="two-icons-desktop">
				<img
					src="https://templesofindia.org/assets/icons/custom_favorite.svg"
					alt=""
					class="visted-img"
				/>
				<span>Favourite</span>
			</div>
		</div>
	</div>

	<!-- details container for desktop and mobile view -->

	<div class="bottom-container">
		<div class="left-container">
			<div class="mobile-icons">
				<div class="two-icons">
					<img
						src="https://templesofindia.org/assets/icons/custom_visited.svg"
						alt=""
						class="visted-img"
					/>Visited
				</div>
				<div class="two-icons">
					<img
						src="https://templesofindia.org/assets/icons/custom_favorite.svg"
						alt=""
						class="visted-img"
					/>Favourite
				</div>
			</div>
			<div class="mobile-location-details">
				<div class="location">
					<span>Location</span> <button class="edit-details-btn">Edit Details</button>
				</div>

				<p class="address">Tamil Nadu,Coimbatore,India</p>
				<div id="map">
					<iframe
						title="map"
						src="https://www.google.com/maps/embed?pb=!1m17!1m8!1m3!1d2939.642808300775!2d77.01483437088658!3d10.951411485704428!3m2!1i1024!2i768!4f13.1!4m6!3e6!4m0!4m3!3m2!1d10.951326499999999!2d77.0145986!5e0!3m2!1sen!2sin!4v1711531969637!5m2!1sen!2sin"
						width="300"
						height="200"
						style="border:0;"
						allowfullscreen=""
						loading="lazy"
						referrerpolicy="no-referrer-when-downgrade"
					></iframe>
				</div>
				<div>
					<p class="top-line" style="margin-top: 30px;"><span>Open Timings </span></p>
					<p>Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday: 07:00 am - 09:00 am</p>
					<p>Monday, Tuesday, Wednesday, Thursday, Friday, Saturday, Sunday: 07:00 am - 09:00 am</p>
				</div>
				<p class="top-line" style="margin-top: 50px;"><span>Pooja Timings </span></p>
				<p>NO DATA</p>
				<p class="top-line" style="margin-top: 20px;"><span>Other Dieties</span></p>
			</div>
			<div class="drop-downs">
				<button
					class="top-line"
					on:click={() => {
						closeItems('dp1', 'angleDown1', 'angleup1');
					}}
				>
					<span
						><i class="fa-solid fa-angle-down" id="angleDown1"></i>
						<i class="fa-solid fa-angle-up hide-content" id="angleup1"></i>
						Special Features</span
					>
					<i class="fa-solid fa-pen"></i>
				</button>
				<div class="drop-down-details" id="dp1">
					<b style="margin-top: 20px;">Foundation Year</b> <br />
					500-1000 years old<br />
					<p style="margin-top: 20px;"><b>Sthala Tree</b></p>
					<br />
					<b>Theertham</b><br />
					Palsunai, Padma theertham, Sengothai Sunai, Kannimar Sunai, Pasumani Sunai<br />
					<p style="margin-top: 20px;"><b>Ratham</b></p>
					<p style="margin-top: 20px;"><b>Architecture</b></p>
					Dravidian Architecture<br />
					<b style="margin-top: 20px;"> Other Speciality</b><br />
					All merciful Lord Ranganatha appears in a standing form facing east pleasing the mind of His
					devotees.
					<hr />
				</div>
			</div>
			<div class="drop-downs">
				<button
					class="top-line"
					on:click={() => {
						closeItems('dp2', 'angleDown2', 'angleup2');
					}}
				>
					<span
						><i class="fa-solid fa-angle-down" id="angleDown2"></i>
						<i class="fa-solid fa-angle-up hide-content" id="angleup2"></i>Sthala Puran</span
					>
					<i class="fa-solid fa-pen"></i>
				</button>
				<div class="drop-down-details hide-content" id="dp2">
					<p>
						Maharshi Kalava was in penance for a quite number of years to have the darshan of Lord
						Narayana. One Durmadhan, son of a Gandarva Viswasu by name was bathing in the tank with
						his wives. Maharshi Vasishta was returning from Mount Kailash after a darshan of Lord
						Shiva. Seeing the sage, Durmadha’s wives stopped bathing and came out of the tank in
						respect to the sage. But Durmadha continued bathing nude. Angry Vasishta cursed Dhurmada
						to be born a demon. The wives fell at the feet of Sage Vasishta and begged for relief.
						Responding to their prayer, sage said that their husband would be back to them in a
						short time.
					</p>
					<p>
						Durmadha wandering here and there as a demon saw Maharshi Kalava and began to harass
						him. Rishi prayed to Lord Narayana for protection. Lord granted darshan to Rishi and
						controlled the demon. With the touch of Lord, Durmadha was relieved of his curse. It is
						believed that this event took place here.
					</p>
					<p>
						The other story is that a king Nanda Boopala, ruling this region renounced his kingdom
						and set out for penance on Lord Narayana. His son Darma Gupta became the king and was
						ruling the region righteously. When he was in the forest for hunting, dusk set in and
						the king could not find the way to the camp. He climbed on a tree and began chanting the
						Gayatri Mantra. A bear, chased by a lion also came to the tree branch and sat along with
						the king.
					</p>
					<p>
						The king said to the bear that both would be at a risk if they returned to the ground.
						The bear suggested that the king may sleep half the night when it would take care of him
						and that it would sleep the remaining night protected by the king. While the king was
						sleeping the lion under the tree asked the bear to push the king down. The bear simply
						said that it could not commit a sin as breach of trust. When the kin woke up and the
						bear started sleeping the lion made the suggestion to the king. Thoughtlessly, the king
						obliged the lion pushing the bear down. Shocked by the behaviour of the king, the bear
						luckily escaping the attack of the lion, cursed the king to become a lunatic. King Nanda
						Boopala seeing the condition of son Darma Gupta, took him to Sage Jaimini for the cure.
						Sage suggested that he should have a dip in Palamalai Theertha and worship Lord
						Ranganatha for recovery. Darma Gupta was thus saved by Palamalai Lord Ranganatha.
					</p>

					<hr />
				</div>
			</div>
			<div class="drop-downs">
				<button
					class="top-line"
					on:click={() => {
						closeItems('dp3', 'angleDown3', 'angleup3');
					}}
				>
					<span
						><i class="fa-solid fa-angle-down" id="angleDown3"></i>
						<i class="fa-solid fa-angle-up hide-content" id="angleup3"></i> Architecture</span
					>
					<i class="fa-solid fa-pen"></i>
				</button>
				<div class="drop-down-details hide-content" id="dp3">
					<p>
						All merciful Lord Ranganatha appears in a standing form facing east pleasing the mind of
						His devotees. Thumbikkai Azhwar and Mother grace the devotees from their respective
						shrines. Adequate space is created around the temple to facilitate car festival and
						movement of devotees during festival times. Many visit the temple frequently as the
						environment and the climate are helpful to keep them healthy and free from any disease.
						Irulars, a tribal community are living near the temple. The car of the temple is
						aesthetically made by skilled craftsmen.

						<br />The devotee crowd is huge on new moon days and Saturdays. There are shrines for
						Lord Vinayaka, Sri Anjaneya and Acharya Sri Ramanuja.
					</p>
					<hr />
				</div>
			</div>
			<div class="drop-downs">
				<button
					class="top-line"
					on:click={() => {
						closeItems('dp4', 'angleDown4', 'angleup4');
					}}
				>
					<span
						><i class="fa-solid fa-angle-down" id="angleDown4"></i>
						<i class="fa-solid fa-angle-up hide-content" id="angleup4"></i> Alankar of Deity</span
					>
					<i class="fa-solid fa-pen"></i>
				</button>
				<div class="drop-down-details hide-content" id="dp4">
					<p></p>
					<hr />
				</div>
			</div>
			<div class="drop-downs">
				<button
					class="top-line"
					on:click={() => {
						closeItems('dp5', 'angleDown5', 'angleup5');
					}}
				>
					<span
						><i class="fa-solid fa-angle-down" id="angleDown5"></i>
						<i class="fa-solid fa-angle-up hide-content" id="angleup5"></i> Prayers and Benefits</span
					>
					<i class="fa-solid fa-pen"></i>
				</button>
				<div class="drop-down-details hide-content" id="dp5">
					<b>Special Vratas and Prayers</b><br />
					Those facing the impact of some curses pray for relief.<br />

					<p style="margin-top: 30px;"><b>Offerings to Deity</b></p>
					<br />
					Devotees perform Tirumanjanam to Lord and Mother with sweet pudding-sarkarai pongal nivedhana.
					<br />
					<p style="margin-top: 30px;"><b>Stotras and Mantras</b></p>
					<br />
					<hr />
				</div>
			</div>
			<div class="drop-downs">
				<button
					class="top-line"
					on:click={() => {
						closeItems('dp6', 'angleDown6', 'angleup6');
					}}
				>
					<span
						><i class="fa-solid fa-angle-down" id="angleDown6"></i>
						<i class="fa-solid fa-angle-up hide-content" id="angleup6"></i>Festivals</span
					>
					<i class="fa-solid fa-pen"></i>
				</button>
				<div class="drop-down-details hide-content" id="dp6">
					<p>Car festival is celebrated in the temple on Chitra Poornima day in April-May.</p>
					<hr />
				</div>
			</div>
			<div class="drop-downs">
				<button
					class="top-line"
					on:click={() => {
						closeItems('dp7', 'angleDown7', 'angleup7');
					}}
				>
					<span
						><i class="fa-solid fa-angle-down" id="angleDown7"></i>
						<i class="fa-solid fa-angle-up hide-content" id="angleup7"></i>Sodasha Upcharas</span
					>
					<i class="fa-solid fa-pen"></i>
				</button>
				<div class="drop-down-details hide-content" id="dp7">
					<p></p>
					<hr />
				</div>
			</div>
			<div class="drop-downs">
				<button
					class="top-line"
					on:click={() => {
						closeItems('dp8', 'angleDown8', 'angleup8');
					}}
				>
					<span
						><i class="fa-solid fa-angle-down" id="angleDown8"></i>
						<i class="fa-solid fa-angle-up hide-content" id="angleup8"></i>Prasadhas</span
					>
					<i class="fa-solid fa-pen"></i>
				</button>
				<div class="drop-down-details hide-content" id="dp8">
					<p></p>
					<hr />
				</div>
			</div>
			<div class="drop-downs">
				<button
					class="top-line"
					on:click={() => {
						closeItems('dp9', 'angleDown9', 'angleup9');
					}}
				>
					<span
						><i class="fa-solid fa-angle-down" id="angleDown9"></i>
						<i class="fa-solid fa-angle-up hide-content" id="angleup9"></i> Social Activities</span
					>
					<i class="fa-solid fa-pen"></i>
				</button>
				<div class="drop-down-details hide-content" id="dp9">
					<p>
						<b>Annadhan</b><br />
						<b>Marriage</b><br />
						<b>Ear Boring</b><br />
						<b>Head Shave</b><br />
						<b>Danaas</b><br />
						<b>Education Facilities</b><br />
						<b> Social Drives</b><br />
						<b> Other Activities </b><br />
					</p>
					<hr />
				</div>
			</div>
			<div class="drop-downs">
				<button
					class="top-line"
					on:click={() => {
						closeItems('dp10', 'angleDown10', 'angleup10');
					}}
				>
					<span
						><i class="fa-solid fa-angle-down" id="angleDown10"></i>
						<i class="fa-solid fa-angle-up hide-content" id="angleup10"></i> Arjita Seva
					</span>
					<i class="fa-solid fa-pen"></i>
				</button>
				<div class="drop-down-details hide-content" id="dp10">
					<p></p>
					<hr />
				</div>
			</div>
			<div>
				<button
					class="top-line"
					on:click={() => {
						displaybutton();
					}}
				>
					<span> Tags </span>
					<i class="fa-solid fa-pen"></i>
				</button>
				<div id="submitBtn" class="submit-btn">
					<hr />
					<button class="submit-button">Submit Changes</button>
				</div>
			</div>
		</div>

		<div class="right-container">
			<div>
				<div class="desktop-location-view">
					<p class="top-line"><span>Location</span> <i class="fa-solid fa-pen"></i></p>
					<a
						href="https://www.google.com/maps/dir//10.9513265,77.0145986/@10.9513265,77.0145986,18z"
						target="_blank"
						class="view-on-maps">View on Maps</a
					>
					<p class="address">Unnamed Road, Anbu Nagar, Podanur, Coimbatore, Tamil Nadu 641023</p>
					<div id="map">
						<iframe
							title="map"
							src="https://www.google.com/maps/embed?pb=!1m17!1m8!1m3!1d2939.642808300775!2d77.01483437088658!3d10.951411485704428!3m2!1i1024!2i768!4f13.1!4m6!3e6!4m0!4m3!3m2!1d10.951326499999999!2d77.0145986!5e0!3m2!1sen!2sin!4v1711531969637!5m2!1sen!2sin"
							width="300"
							height="250"
							style="border:0;"
							allowfullscreen=""
							loading="lazy"
							referrerpolicy="no-referrer-when-downgrade"
						></iframe>
					</div>
					<div class="open-timings">
						<p class="top-line"><span>Open Timings</span> <i class="fa-solid fa-pen"></i></p>
						<p>Alldays: 07:00 am - 09:00 am</p>
						<p>Alldays: 07:00 am - 09:00 am</p>
					</div>
					<p class="top-line"><span>Pooja Timings </span><i class="fa-solid fa-pen"></i></p>
					<p class="top-line"><span>Other Dieties</span><i class="fa-solid fa-pen"></i></p>
				</div>
				<div>
					<div class="sub-list">
						<p class="top-line"><span>Amenities</span> <i class="fa-solid fa-pen"></i></p>
						<ul class="checklist">
							<li><i class="fa-solid fa-check"></i> Drinking Water</li>
							<li><i class="fa-solid fa-check"></i> Pooja Items Shops</li>
							<li><i class="fa-solid fa-check"></i> Restaurants Nearby</li>
							<li><i class="fa-solid fa-check"></i> Restroom</li>
						</ul>
					</div>
					<div>
						<p class="top-line"><span>How to reach?</span> <i class="fa-solid fa-pen"></i></p>
						<p class="travel-list-item">
							<b>Nearest Bus Station </b><i class="fa-solid fa-bus travel"></i>
						</p>
						<p>Gandhipuram</p>
						<p class="travel-list-item">
							<b>Nearest Railway Stattion </b><i class="fa-solid fa-train travel"></i>
						</p>
						<p>Coimbatore</p>
						<p class="travel-list-item">
							<b>Nearest Airport </b><i class="fa-solid fa-plane-up travel"></i>
						</p>
						<p>Coimbatore</p>
					</div>
					<div>
						<p class="top-line"><span>Contact Details </span><i class="fa-solid fa-pen"></i></p>
						<p>Name</p>
						<p>Phone<br /> +91-94433 48564</p>
						<p>Name</p>
						<p>Phone <br /> +91-94433 48564</p>
						<p>Website</p>
					</div>
				</div>
			</div>
		</div>
	</div>

	<div class="mobile-desktop-view-details">
		<div class="sub-list">
			<p class="top-line"><span>Amenities</span> <i class="fa-solid fa-pen"></i></p>
			<ul class="checklist">
				<li><i class="fa-solid fa-check"></i> Drinking Water</li>
				<li><i class="fa-solid fa-check"></i> Pooja Items Shops</li>
				<li><i class="fa-solid fa-check"></i> Restaurants Nearby</li>
				<li><i class="fa-solid fa-check"></i> Restroom</li>
			</ul>
		</div>
		<div>
			<p class="top-line"><span>How to reach?</span> <i class="fa-solid fa-pen"></i></p>
			<div class="travel-item">
				<p class="travel-list-item">
					<b>Nearest Bus Station </b><i class="fa-solid fa-bus travel"></i>
				</p>
				<p>Gandhipuram</p>
			</div>
			<div class="travel-item">
				<p class="travel-list-item">
					<b>Nearest Railway Stattion </b><i class="fa-solid fa-train travel"></i>
				</p>
				<p>Coimbatore</p>
			</div>
			<div class="travel-item">
				<p class="travel-list-item">
					<b>Nearest Airport </b><i class="fa-solid fa-plane-up travel"></i>
				</p>
				<p>Coimbatore</p>
			</div>
		</div>
		<div>
			<p class="top-line"><span>Contact Details </span><i class="fa-solid fa-pen"></i></p>
			<p>Name</p>
			<p>Phone<br /> +91-94433 48564</p>
			<p>Name</p>
			<p>Phone <br /> +91-94433 48564</p>
			<p>Website</p>
		</div>
	</div>

	<div style="margin-top: 15px;">
		<hr />
		<button class="top-line last-lines">
			<span> Contributors </span>
		</button>
	</div>
	<hr />
	<div>
		<button class="top-line last-lines">
			<span> Comments </span>
		</button>
	</div>

	<!-- footer -->

	<footer>
		<div class="sub-footer">
			<div>
				<img
					src="https://templesofindia.org/assets/images/tofi_logo/tofi-logo_navbar.png"
					alt="logo"
				/>
				<p>Temples of India</p>
				<p>World's Largest Hindu Temples Portal.</p>
			</div>
			<div>
				<a href="">Quick Links</a><br />
				<a href="https://templesofindia.org/">Home</a><br />
				<a href="https://templesofindia.org/ourVision"> About Us</a><br />
				<a href="https://templesofindia.org/nearbyTemples"> Nearby Temples </a><br />
				<a href="https://play.google.com/store/apps/details?id=com.tofi.app"> Download App </a><br
				/>
				<a href="https://templesofindia.org/donate"> Donate to Us </a>
			</div>
			<div>
				<a href="https://templesofindia.org/searchTemple">Search Temples</a><br />
				<a href="https://youtu.be/4nn8Su_F53g">Watch Video</a><br />
				<a href="https://templesofindia.org/disclaimer"> Disclaimer</a><br />
				<a href="https://blog.templesofindia.org/"> Our Blog </a><br />
				<a href="https://donatefordharma.org/"> Donate for Dharma </a><br />
			</div>
			<div class="social-media">
				<a href="https://www.facebook.com/tofi.fb"><i class="fa-brands fa-facebook-f"></i> </a>
				<a href="https://www.twitter.com/tofi_official"><i class="fa-brands fa-twitter"></i></a>
				<a href="https://www.instagram.com/tofi_in/"><i class="fa-brands fa-instagram"></i></a>
				<a href="https://www.linkedin.com/company/temples-of-india">
					<i class="fa-brands fa-linkedin-in"></i></a
				>
			</div>
		</div>
		<div class="mail">
			<p>©Temples of India 2020-2023 | Email: contact@templesofindia.org</p>
		</div>
	</footer>
</div>

<!-- styles -->
<style>
	* {
		box-sizing: border-box;
		margin: 0px;
		padding: 0px;
	}
	.main-container {
		display: flex;
		flex-direction: column;
	}
	.navbar {
		margin-top: 15px;
		display: flex;
		justify-content: space-around;
		align-items: center;
		font-family: system-ui, 'Segoe UI', 'Open Sans', 'Helvetica Neue', sans-serif;
	}
	.navbar a {
		text-decoration: none;
		font-weight: 400;
		color: black;
	}
	.logo {
		display: flex;
		align-items: center;
	}
	.nav-temple-name {
		font-family: 'Playfair Display' !important;
		font-size: 35px;
	}

	.add-temples {
		height: 15px;
		color: red;
	}
	ul {
		list-style-type: none;
		display: flex;
		justify-content: space-around;
		gap: 25px;
	}
	.temple-image {
		width: 100%;
		margin-top: 25px;
	}
	.bottom-container {
		margin-top: 25px;
		display: flex;
		justify-content: space-around;
		align-items: flex-start;
		width: 100%;
		font-family: system-ui, 'Segoe UI', 'Open Sans', 'Helvetica Neue', sans-serif;
	}
	.visted-img {
		height: 20px;
	}
	.drop-downs {
		padding: 20px;
		display: flex;
		flex-direction: column;
		align-items: flex-start;
		justify-content: space-around;
	}
	#dp2 p {
		margin-bottom: 30px;
	}
	.top-line {
		width: 95%;
		gap: 10px;
		text-align: left;
		background: none;
		outline: none;
		border: none;
		margin-bottom: 20px;
		display: flex;
		justify-content: space-between;
	}
	.top-line span {
		color: #a50740;
		font-weight: 700;
		font-size: 20px;
	}
	.drop-down-details {
		align-self: flex-start;
		padding-left: 5%;
		width: 94%;
		padding: 20px;
	}
	.drop-down-details p {
		padding-bottom: 40px;
	}
	.hide-content {
		display: none;
	}
	.submit-btn {
		display: none;
		margin-top: 40px;
	}
	.submit-button {
		width: 100%;
		margin-top: 10px;
	}
	.display-submit-btn {
		display: block;
	}
	.view-on-maps {
		color: blue;
		font-weight: 500;
		text-decoration: none;
		font-size: 20px;
	}
	.address {
		font-size: 20px;
		font-weight: 500;
	}
	.open-timings {
		padding: 10px;
		padding-top: 20px;
	}
	.checklist {
		padding: 15px;
		list-style-type: none;
		display: flex;
		flex-direction: column;
		align-items: flex-start;
	}
	.checklist li i {
		color: green;
		font-size: 24px;
		padding-right: 5px;
	}
	.travel-item {
		padding-bottom: 25px;
	}
	.travel-list-item {
		display: flex;
		justify-content: space-between;
		align-self: flex-start;
		width: 95%;
	}
	.travel {
		color: #a50740;
	}
	footer {
		background-color: rgb(255, 226, 64);
		color: #a50740;
		width: 100%;
		font-family: system-ui, 'Segoe UI', 'Open Sans', 'Helvetica Neue', sans-serif;
		font-weight: 400;
		gap: 20px;
	}
	footer .social-media i {
		color: rgb(110, 110, 240);
		padding: 6px;
		font-size: 30px;
	}
	footer .mail {
		background-color: rgb(227, 204, 76);
		min-width: 100%;
	}
	.drop-down-details hr {
		min-width: 100%;
		margin-top: 20px;
	}
	.sub-footer div a {
		text-decoration: none;
		color: #a50740;
		padding: 25px;
		gap: 30px;
		font-weight: 400;
		font-size: 18px;
	}
	.last-lines {
		padding: 10px;
	}
	@media (max-width: 850px) {
		.navbar,
		.right-container {
			display: none;
		}
		.mobile-nav {
			display: flex;
			align-items: center;
			justify-content: space-around;
		}
		.off-canvas {
			display: flex;
			flex-direction: column;
		}
		#closeBtn {
			align-self: flex-end;
			padding: 10px;
			margin: 10px;
			gap: 10px;
		}
		.profile-details {
			display: flex;
			align-items: center;
			justify-content: flex-start;
			padding: 20px;
			gap: 10px;
		}
		.sidebar-item {
			display: flex;
			justify-content: flex-start;
			align-items: center;
			padding: 15px;
			gap: 10px;
		}
		.sidebar {
			width: 80%;
		}
		.sidebar div i {
			color: #a50740;
		}
		.cross-btn {
			background: none;
			border: none;
		}
		.profile-img {
			height: 50px;
			border-radius: 10px;
		}
		.left-container {
			padding: 20px;
		}
		.desktop-location-view {
			display: none;
		}
		.bottom-container {
			flex-direction: column;
		}
		.mobile-icons {
			display: flex;
			align-items: flex-end;
			justify-content: flex-end;
		}
		.mobile-location-details {
			display: flex;
			flex-direction: column;
			align-items: flex-start;
			justify-content: flex-start;
		}
		.mobile-desktop-view-details {
			width: 100%;
			display: flex;
			flex-direction: column;
			padding: 20px;
		}

		.two-icons {
			display: flex;
			flex-direction: column;
			gap: 20px;
		}
		.location {
			margin-top: 25px;
			width: 100%;
			display: flex;
			align-items: center;
			justify-content: space-between;
			text-align: left;
			color: #a50740;
		}
		.location span {
			font-weight: 700;
			font-size: 20px;
		}
		.edit-details-btn {
			background-color: white;
			border: 1px black solid;
			border-radius: 25px;
			padding: 6px;
			font-weight: 500;
			box-shadow: 0px 2px 0px 0px;
		}

		footer {
			display: flex;
			flex-direction: column;
		}
		footer div {
			padding: 15px;
		}
	}
	@media (min-width: 851px) {
		.mobile-nav,
		.mobile-location-details,
		.mobile-icons,
		.sidebar,
		.mobile-desktop-view-details {
			display: none;
		}
		.left-container {
			display: flex;
			flex-direction: column;
			width: 65%;
			padding: 25px;
		}
		.right-container {
			width: 30%;
			display: flex;
			flex-direction: column;
			background-color: rgb(245, 244, 244);
			padding: 10px;
		}
		.icons {
			display: flex;
			align-items: center;
			justify-content: flex-end;
			padding-right: 20px;
		}
		.two-icons-desktop {
			display: flex;
			flex-direction: column;
			gap: 10px;
			padding: 10px;
		}
		footer {
			display: flex;
			flex-direction: column;
		}
		footer .sub-footer {
			display: flex;
			justify-content: space-around;
			padding: 10px;
		}
		footer .mail {
			align-self: center;
			justify-self: center;
			padding: 15px;
			text-align: center;
		}
	}
</style>

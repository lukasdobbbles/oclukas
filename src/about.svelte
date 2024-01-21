<script>
	let project_list = [
		{
			name: "Propel.io",
			icon: "propel.io_icon.webp",
			screenshot: "propel.io_screenshot.webp",
			comment: "multiplayer unity game where you push people off the map",
			link: "https://apps.apple.com/tr/app/propel-io/id6450183559",
		},
		{
			name: "Progeny",
			screenshot: "progeny.png",
			comment: "a minimalist, clean programming language",
			link: "https://github.com/PoseidonCoder/progeny",
		},
		{
			name: "RoSniperX",
			screenshot:
				"https://greasyfork.s3.us-east-2.amazonaws.com/im9fci8wp0mqdazgmmt4qmuhjede",
			comment:
				"join any player in Roblox regardless if they're your friend or not (11,196+ downloads) ",
			link: "https://greasyfork.org/en/scripts/464350-rosniperx",
		},
	];
</script>

<div id="about" class="section">
	<h2>About me</h2>
	<p class="block-text">
		Hello! My name is Lukas Dobbles and I'm a sophomore in high school. This
		was made for my Video Production class to showcase my work. I would've
		liked to have made this page in pure HTML, CSS, and JS but these
		school-distributed computers are very limited in what they can do, and
		editing a text/html file is one of those limitations. As can be seen,
		I'm an avid tech enthusiast and always trying to educate myself on
		technology/engineering so that I can eventually become independently
		wealthy. I would derive this technocratic/entrepreneurship view of the
		world from my dad. He plays a huge role in my life, whether project
		ideas or school-related. While I like to focus on the
		engineering/programming aspects of technology I consider Video
		Production an accessory of my technology-related skills. I have two
		YouTube channels. One has over twenty-one thousand views on one video
		but I unfortunately lost that account. My new account is just where I
		generate auto-generated YouTube short content daily. It's not doing as
		well as my first account but I'm hoping that by creating a script that
		posts videos twice a day I can beat the YouTube algorithm and make a
		little bit of money.
	</p>

	<h2>Skills</h2>
	<p class="block-text">
		HTML, CSS, JS, React, Unity, C#, Python, React, React Native, NextJS,
		Raspberry Pi, Golang, Lua (Roblox)
	</p>

	<h2>Projects</h2>
	<div class="projects-grid">
		{#each project_list as project}
			<div class="card">
				<div class="card-text">
					{project.name}
					{#if project.icon}
						<img
							src={project.icon}
							alt={project.icon}
							class="project-icon"
						/>
					{/if}
				</div>

				<img
					src={project.screenshot}
					alt={project.screenshot}
					class="card-image"
				/>

				<p class="card-comment block-text">
					{project.comment}
				</p>

				<a href={project.link} target="_blank" class="button">
					<span>View Project</span>
				</a>
			</div>
		{/each}
	</div>
</div>

<script lang="ts">
	import windows11Wallpaper from '$lib/assets/windows11.png';
	import cloud from '$lib/assets/icons/cloud.svg';
	import windows from '$lib/assets/icons/windows.svg';
	import search from '$lib/assets/icons/search.svg';
	import windowManager from '$lib/assets/icons/desktop-manager.svg';
	import chat from '$lib/assets/icons/chat.svg';
	import fileExplorer from '$lib/assets/icons/file-explorer.svg';
	import edge from '$lib/assets/icons/microsoft-edge.svg';

	import overflow from '$lib/assets/icons/overflow.svg';
	import wifi from '$lib/assets/icons/wifi.svg';
	import battery from '$lib/assets/icons/battery.svg';
	import volume from '$lib/assets/icons/volume.svg';
</script>

<div class="relative w-full h-screen">
	<img
		class="w-full h-screen object-cover absolute top-0 left-0 -z-10"
		src={windows11Wallpaper}
		alt="windows wallpaper"
	/>

	<!-- bottom navigation -->
	<div
		class="absolute bottom-0 w-full bg-[rgba(68,68,68,0.3)] backdrop-blur-[35px] px-7 py-1 flex items-center justify-between"
	>
		<div class="flex gap-2">
			<img src={cloud} alt="" />
			<div class="text-white text-xs flex flex-col gap-1 font-normal">
				<span class="flex"
					>8
					<svg
						xmlns="http://www.w3.org/2000/svg"
						width="4"
						height="5"
						viewBox="0 0 4 5"
						fill="none"
						class="self-center ml-[3px] -mt-1"
					>
						<circle cx="2" cy="2.25" r="1.5" stroke="white" />
					</svg>C</span
				>
				<span>Partly sunny</span>
			</div>
		</div>

		<div class="flex gap-4">
			<img
				src={windows}
				alt=""
				class="hover:cursor-pointer transition-all duration-150 hover:bg-[rgba(68,68,68,0.5)] inset-1 drop-shadow-md p-2 rounded-sm"
			/>
			<img
				src={search}
				alt=""
				class="hover:cursor-pointer transition-all duration-150 hover:bg-[rgba(68,68,68,0.5)] inset-1 drop-shadow-md p-2 rounded-sm"
			/>
			<img
				src={windowManager}
				alt=""
				class="hover:cursor-pointer transition-all duration-150 hover:bg-[rgba(68,68,68,0.5)] inset-1 drop-shadow-md p-2 rounded-sm"
			/>
			<img
				src={chat}
				alt=""
				class="hover:cursor-pointer transition-all duration-150 hover:bg-[rgba(68,68,68,0.5)] inset-1 drop-shadow-md p-2 rounded-sm"
			/>
			<img
				src={fileExplorer}
				alt=""
				class="hover:cursor-pointer transition-all duration-150 hover:bg-[rgba(68,68,68,0.5)] inset-1 drop-shadow-md p-2 rounded-sm"
			/>
			<img
				src={edge}
				alt=""
				class="hover:cursor-pointer transition-all duration-150 hover:bg-[rgba(68,68,68,0.5)] inset-1 drop-shadow-md p-2 rounded-sm"
			/>
		</div>

		<div class="flex items-center gap-[10px]">
			<img src={overflow} alt="" />
			<div class="flex gap-2">
				<img src={wifi} alt="" />
				<img src={volume} alt="" />
				<img src={battery} alt="" />
			</div>
			<div class="text-white flex text-xs flex-col font-light text-right">
				<span>11:00 AM</span>
				<span>10/05/2023</span>
			</div>
		</div>
	</div>
</div>

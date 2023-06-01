<script lang="ts">
	const people = [
		{
			photo:
				'https://cdn.discordapp.com/attachments/1107308201969459212/1107308277324329090/b12b3edb7d033205.jpg',
			instagram: 'clydinite',
			name: '郭彥均',
			position: '社長',
			description:
				'你好，我是資訊研究社的創社社長郭彥均。從我上國小的時候開始，我對程式設計便產生了濃厚的興趣。然而，在進入高師大附中之後，我意識到學校並沒有一個與程式設計相關的社團存在。儘管我對社團的經營毫無經驗，但我仍決心在這個學校開創一個屬於我們資訊人的世界，歡迎你的加入！'
		},
		{
			photo:
				'https://cdn.discordapp.com/attachments/1107308201969459212/1107308279937380463/cc84907753317cbf.jpg',
			instagram: 'sam317901',
			name: '李嘉峰',
			position: '副社長',
			description:
				'大家好，我是李嘉峰，我擔任副社長，但我只會寫一點點的Python跟Javascript……，還有，我平常的興趣是寫程式和打排球，非常歡迎大家來跟我討論各式各樣的東西，本人涉略挺廣，就是樣樣不精（呵呵），從股票、攝影、素描、電繪都有涉獵。也可以經常看到我被其他幹部電在地板爬（是真的被電喔，不過那是因為我喜歡接電路）。'
		},
		{
			photo:
				'https://cdn.discordapp.com/attachments/1107308201969459212/1107308277953482863/f8f55c58c888f0c3.jpg',
			instagram: 'benson0710908',
			name: '林恩嶙',
			position: '公關',
			description:
				'嗨大家好我是恩嶙，高二加入附中第一屆資研社就不知道為什麼變幹部了，然後我真的超廢，不要再說我是電神了，平常沒什麼時間發展興趣，就讀個書搞個社團，然後空閒時間就沒了，物理也沒有很強，但是還是想考物理系，然後加入資研社認識了這個領域還有一堆電神我覺得很棒。希望學弟妹可以加資研社或是多多參與資訊領域活動，增加附中CS的風氣。'
		},
		{
			photo:
				'https://cdn.discordapp.com/attachments/1107308201969459212/1107308278276435968/14470d5764f6c939.jpg',
			instagram: 'kaiyuanee',
			name: '張凱垣',
			position: '教學',
			description:
				'你好，我是張凱垣，嚴格來講我是資訊研究社副教學。雖然HTML、CSS、JS是社團課程的主要內容，但我比較熟悉的語言反而是Python, C++和Java這些競賽程式語言。我的Discord是KaiYuanee#9165，平常喜歡玩的遊戲是Minecraft。歡迎你們聯繫我的IG或Discord騷擾我。'
		},
		{
			photo:
				'https://cdn.discordapp.com/attachments/1107308201969459212/1107308277680832562/d27454ed6f2b5c3a.png',
			instagram: 'hsiaocheng1106',
			name: '蕭政佑',
			position: '總務',
			description:
				'大家好，我是蕭政佑，我是擔任總務（雖然沒什麼活動支出），目前會的程式語言比較熟的是JavaScript與Python，這學期有和學生會合作網站。平常興趣有寫程式，也會打電動，在課業或程式上有問題也可以來問我歡迎與我交流，有什麼不懂也可以問，請大家多多指教。'
		},
		{
			photo:
				'https://cdn.discordapp.com/attachments/1107308201969459212/1107308279245328475/7d6948e354e5f38d.jpg',
			instagram: 'dannielsu',
			name: '蘇群展',
			position: '活動',
			description:
				'早安你好我叫蘇群展，我是附中資研社活動。剛好有榮幸能當到資研社社幹鼻祖，深感驕傲。平常的興趣就打球運動打電動，但若是說到程式的部分，我只能是深感不如，有太多東西還需要我去探索學習。歡迎更多的人再來加入我們一起Coding！'
		},
		{
			photo:
				'https://cdn.discordapp.com/attachments/1107308201969459212/1107308280331632761/61f1e286a96421bd.jpg',
			instagram: 'yanshuo_huang',
			name: '黃彥碩',
			position: '活動',
			description: '好欸我是黃彥碩，好欸好欸這是我的自介，謝謝大家。'
		}
	];
</script>

<div class="grid md:grid-cols-2 md:gap-12">
	{#each people as person}
		<div class="py-4 md:py-0">
			<img class="md:rounded-lg aspect-[3/4] object-cover" src={person.photo} alt={person.name} />
			<div class="flex items-baseline py-4">
				<p class="m-3 text-2xl font-bold">{person.name}</p>
				<p class="m-3 text-lg">{person.position}</p>
				<a class="m-3 text-lg underline" href={`https://www.instagram.com/${person.instagram}`}
					>@{person.instagram}</a
				>
			</div>
			<p class="m-3 mt-0 text-xl">
				{person.description}
			</p>
		</div>
	{/each}
</div>


<template>
	<div class="container">
		<div class="pt-5 relative" >
			<div id="particles-js" style="height: 200px;"></div>
			<div class="vertical-center title">
				<h1 class="title">スタッフ紹介</h1>
                <p class="title">staff</p>
			</div>
		</div>
        <div>
            <b-container>
                <b-row class="px-2 mx-auto d-flex align-items-center">
                    <b-col class="pr-0 pl-0" cols="4">
                        <img class="max-img" src="/img/daichi.jpg" alt="Responsive image">
                        <p class="pop mt-3 mb-0">代表</p>
                        <h4 class="pop mb-0">木下大地</h4>
                        <h6 class="pop mt-0">DaichiKinoshita</h6>
                    </b-col>
                    <b-col class="pl-0 pr-1">
                        <div class="pop sm-txt">
                            <table class="mx-auto">
                                <tr>
                                    <th class="align-left xs-txt blue-txt py-2">Birthday/誕生日</th>
                                    <td class="align-left pl-2 main-font">H3.12月30日</td>
                                </tr>
                                <hr class="m-0">
                                <tr>
                                    <th class="align-left xs-txt blue-txt py-2">Hobby/趣味</th>
                                    <td class="align-left pl-2 main-font">ボードゲーム</td>
                                </tr>
                                <hr class="m-0">
                                <tr>
                                    <th class="align-left xs-txt blue-txt py-2">Specialty/特技</th>
                                    <td class="align-left pl-2 main-font">料理</td>
                                </tr>
                                <hr class="m-0">
                                <tr>
                                    <th class="align-left xs-txt blue-txt py-2">Favorite/好きな物</th>
                                    <td class="align-left pl-2 main-font">ラーメン</td>
                                </tr>
                                <hr class="m-0">
                                <tr>
                                    <th class="align-left xs-txt blue-txt py-2">Skill/スキル</th>
                                    <td class="align-left pl-2 main-font">Js C++ クラウド技術 etc..</td>
                                </tr>
                                <hr class="m-0">
                                <tr>
                                    <th class="align-left xs-txt blue-txt py-2">Ambition/野望</th>
                                    <td class="align-left pl-2 main-font">日本をシリコンバレーにする</td>
                                </tr>
                                <hr class="m-0">
                                <tr>
                                    <th class="align-left xs-txt blue-txt py-2">Message/メッセージ</th>
                                    
                                    <td class="align-left pl-2 main-font">豊富なビジネス経験に<br>自信があります！<br>なんでもご相談ください！</td>
                                </tr>
                                <hr class="m-0">
                            </table>
                        </div>
                    </b-col>
                </b-row>
            </b-container>
        </div>
		<div class="relative menu-container">
			<div class="vertical-center">
				<nav class="menu">
					<input type="checkbox" href="#" class="menu-open" name="menu-open" id="menu-open" v-on:change="onMenuStateChange"/>
					<label class="menu-open-button" for="menu-open">
						<span class="hamburger hamburger-1"></span>
						<span class="hamburger hamburger-2"></span>
						<span class="hamburger hamburger-3"></span>
					</label>
					<a href="#" class="menu-item" id="menu-1"> <i class="fa fa-question"></i> </a>
					<b-popover ref="popover1" target="menu-1" triggers="focus" placement="top">
						<template v-slot:title>what's valuup</template>
						<b>valuup</b>とは
					</b-popover>
					<a href="#" class="menu-item" id="menu-2"> <i class="fas fa-hammer"></i> </a>
					<b-popover ref="popover2" target="menu-2" triggers="focus" placement="topright">
						<template v-slot:title>develop</template>
						開発実績
					</b-popover>
					<a href="#" class="menu-item" id="menu-3"> <i class="fa fa-user"></i> </a>
					<b-popover ref="popover3" target="menu-3" triggers="focus" placement="bottomright">
						<template v-slot:title>staff</template>
						スタッフ紹介
					</b-popover>
					<a href="#" class="menu-item" id="menu-4"> <i class="fa fa-envelope"></i> </a>
					<b-popover ref="popover4" target="menu-4" triggers="focus" placement="bottom">
						<template v-slot:title>contact</template>
						お問い合わせ
					</b-popover>
					<a href="#" class="menu-item" id="menu-5"> <i class="fas fa-building"></i> </a>
					<b-popover ref="popover5" target="menu-5" triggers="focus" placement="bottomleft">
						<template v-slot:title>company</template>
						会社概要
					</b-popover>
					<a href="#" class="menu-item" id="menu-6"> <i class="fas fa-blog"></i> </a>
					<b-popover ref="popover6" target="menu-6" triggers="focus" placement="topleft">
						<template v-slot:title>blog</template>
						ブログ
					</b-popover>
				</nav>
				<!-- filters -->
				<svg xmlns="http://www.w3.org/2000/svg" version="1.1">
					<defs>
						<filter id="shadowed-goo">
								<feGaussianBlur in="SourceGraphic" result="blur" stdDeviation="10" />
								<feColorMatrix in="blur" mode="matrix" values="1 0 0 0 0  0 1 0 0 0  0 0 1 0 0  0 0 0 18 -7" result="goo" />
								<feGaussianBlur in="goo" stdDeviation="3" result="shadow" />
								<feColorMatrix in="shadow" mode="matrix" values="0 0 0 0 0  0 0 0 0 0  0 0 0 0 0  0 0 0 1 -0.2" result="shadow" />
								<feOffset in="shadow" dx="1" dy="1" result="shadow" />
								<feComposite in2="shadow" in="goo" result="goo" />
								<feComposite in2="goo" in="SourceGraphic" result="mix" />
						</filter>
						<filter id="goo">
								<feGaussianBlur in="SourceGraphic" result="blur" stdDeviation="10" />
								<feColorMatrix in="blur" mode="matrix" values="1 0 0 0 0  0 1 0 0 0  0 0 1 0 0  0 0 0 18 -7" result="goo" />
								<feComposite in2="goo" in="SourceGraphic" result="mix" />
						</filter>
					</defs>
				</svg>
			</div>
		</div>
		<div>
		</div>
	</div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import particles from '~/static/js/set.mjs'

export default {
	components: {
		Logo
	},
	mounted(){
		particlesJS('particles-js',particles);
    },
    beforeDestroy() {
		for(let i=0; i<this.timeoutIds.length; i++){
			if(this.timeoutIds[i]){
				clearTimeout(this.timeoutIds[i]);
			}
		}
	},
	data: ()=>({
		menuChecked:false,
		timeoutIds:[
			null,
			null,
			null,
			null,
			null,
			null,
		]
	}),
	methods: {
		onMenuStateChange(e){
			this.menuChecked = e.srcElement.checked
			if(this.menuChecked){
				this.timeoutIds[0] = setTimeout(()=>{
					if(this.menuChecked){
						this.$refs.popover1.$emit('open')
					}
				},600)
				this.timeoutIds[1] = setTimeout(()=>{
					if(this.menuChecked){
						this.$refs.popover2.$emit('open')
					}
				},1100)
				this.timeoutIds[2] = setTimeout(()=>{
					if(this.menuChecked){
						this.$refs.popover3.$emit('open')
					}
				},1100)
				this.timeoutIds[3] = setTimeout(()=>{
					if(this.menuChecked){
						this.$refs.popover4.$emit('open')
					}
				},600)
				this.timeoutIds[4] = setTimeout(()=>{
					if(this.menuChecked){
						this.$refs.popover5.$emit('open')
					}
				},1600)
				this.timeoutIds[5] = setTimeout(()=>{
					if(this.menuChecked){
						this.$refs.popover6.$emit('open')
					}
				},1600)
			}else{
				this.$refs.popover1.$emit('close')
				this.$refs.popover2.$emit('close')
				this.$refs.popover3.$emit('close')
				this.$refs.popover4.$emit('close')
				this.$refs.popover5.$emit('close')
				this.$refs.popover6.$emit('close')
				for(let i=0; i<this.timeoutIds.length; i++){
					if(this.timeoutIds[i]){
						clearTimeout(this.timeoutIds[i]);
					}
				}
			}
		}
	}
}
</script>

<style lang="scss">
</style>

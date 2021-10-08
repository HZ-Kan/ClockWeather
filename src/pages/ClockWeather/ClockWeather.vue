<template>
    <div class="CW">
        <div style="--i:1;" class="CW_container">
	        <span>7</span>
        </div>
        <div style="--i:2;" class="CW_container">
	        <span>8</span>
        </div>
        <div style="--i:3;" class="CW_container">
	        <span>9</span>
        </div>
        <div style="--i:4;" class="CW_container"> 
	        <span>10</span>
        </div>
        <div style="--i:5;" class="CW_container">
	        <span>11</span>
        </div>
        <div style="--i:6;" class="CW_container">
	        <span>12</span>
        </div>
        <div style="--i:7;" class="CW_container">
	        <span>1</span>
        </div>
        <div style="--i:8;" class="CW_container">
	        <span>2</span>
        </div>
        <div style="--i:9;" class="CW_container">
	        <span>3</span>
        </div>
        <div style="--i:10;" class="CW_container">
	        <span>4</span>
        </div>
        <div style="--i:11;" class="CW_container">
	        <span>5</span>
        </div>
        <div style="--i:12;" class="CW_container">
	        <span>6</span>
        </div>
        <div class="clock">00:00:00</div>
    </div>
</template>


<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		methods: {

		}
	}
</script>

<style scoped>
.CW{
    width: 80vw;
    height: 80vw;
    position: relative;
    background: #eee;
    border-radius: 50%;
}
.CW .CW_container{
    position: absolute;
    left: 50%;
    top: 50%;
    color: white;
    font-size: 6vw;
    text-shadow: 0 0 5px black;
}
.CW span{
    position: absolute;
    transform: rotate(0);

}
.CW .CW_container{
    transform: rotateZ(calc(var(--i) * 30deg)) translateY(40vw);
}
.CW .CW_container span{
    transform: rotateZ(calc(var(--i) * -30deg));
}

.clock{
    position: absolute;
    font-size: 6vw;
    left: 50%;
    top: 60%;
    transform: translateX(-50%);
    color: #1e90ff;
    background: black;
    padding: 1.5vw;
    border-radius: 1.5vw;
}
	
</style>

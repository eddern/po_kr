<script>
	import { smallBlind, bigBlind, nextBigBlind, nextSmallBlind } from 'gameStore';
</script>

<style>
	mainWrapper {
		width: 50%;
	}

	blindsWrapper {
		width: 200px;
		display: flex;
		width: 100%;
		justify-content: space-around;
	}

	blindNumber {
		font-size: 12rem;
		font-weight: 200;
		width: 50%;
		text-align: center;
		color: #ddd;
		margin: 0;
	}

	nextBlindNumber {
		color: #666;
		font-size: 6rem;
		font-weight: 100;
		width: 50%;
		text-align: center;
		margin: 0;
	}
	h3 {
		color: #aaa;
		font-weight: 100;
		font-size: 2rem;
		margin: 0;
	}
</style>

<mainWrapper>
	<h3>Blinds</h3>
	<blindsWrapper>
		<blindNumber>{$smallBlind}</blindNumber>
		<blindNumber>{$bigBlind}</blindNumber>
	</blindsWrapper>
	<blindsWrapper>
		<nextBlindNumber>{$nextSmallBlind}</nextBlindNumber>
		<nextBlindNumber>{$nextBigBlind}</nextBlindNumber>
	</blindsWrapper>
</mainWrapper>

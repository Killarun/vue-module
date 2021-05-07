<template>
    		<div class="avt-summary-item2 avt-t05-block">
					<div class="avt-t05-block-tags">
						<div class="avt-t05-tag__block">
							<div class="avt-t05-tag avt-t05-tag-text">{{warrenty}}</div>
							<div class="avt-t05-tag__flag-right"></div>
						</div>
						<div class="avt-t05-tag__block">
							<div class="avt-t05-tag__flag-left"></div>
							<div class="avt-t05-tag avt-t05-tag-text">{{tickness}}</div>
							<div class="avt-t05-tag__flag-right"></div>
						</div>
						<div class="avt-t05-tag__block">
							<div class="avt-t05-tag__flag-left"></div>
							<div class="avt-t05-tag avt-t05-tag-text">{{zink}}</div>
							<div class="avt-t05-tag__flag-right--mobile"></div>
						</div>
					</div>

					<div class="avt-t05-box">
						<div class="avt-t05-block__container">
							<p class="avt-t05-block__container-p avt-t05-block__container-title-text"><i class="fal fa-layer-plus avt-t05-block__container-icon"></i>Полиэстер</p>

							<div class="avt-t05-block__container-inline">
								<p class="avt-t05-block__container-p avt-t05-block__container-text">
									Собственное производство<br>
									Профиль с малозаметными стыками на кровле<br>
									Надежная упаковка
								</p>
								<div class="avt-t05-block__container avt-t05-block__container--wight">
									<div class="avt-t05-prodaction-day"><span class="avt-t05-prodaction__text--big"><span class="avt-t05-prodaction__text-day">2</span>&nbsp;дня</span></div>
									<div class="avt-t05-prodaction avt-t05-prodaction__text">срок изготовления<br>вашего заказа</div>
								</div>
							</div>

							<div class="avt-t05-block__price avt-t05-block__price-text"> 
								<div class="avt-t05-block__price-row1">
									<div class="avt-t05-block__price-mob-block">
										<span class="avt-t05-block__price-text--price">Цена</span> 
										<span class="avt-t05-block__price-text--summ avt-t05-block__price-text--price-indent" id="avtid_t05pe-price">490</span> руб/кв.м
									</div>
									<div rel="price" class="avt-t05-block__price-all avt-elem-for-custom-tooltip" title="-" id="avtid_t05pe-price-all">
										<i class="fal fa-tags"></i>&nbsp;&nbsp;&nbsp;ВСЕ ЦЕНЫ
									</div>
								</div>
								<div class="avt-t05-block__price-ot" id="avtid_t05pe-price-ot">
									при покупке от ...
								</div>
							</div>

							
						</div>
						
					</div>
					<div class="avt-summary-item2-line3">
						<button class="avt-button__fix avt-button__fix--green">Сделать расчет</button>
						<button class="avt-button__fix avt-button__fix--white">Консультация</button>
						<!-- <div class="avt-button__fix avt-button__fix--green" onclick="show_form_actions('Полиэстер, глянец (заявка с лендинга Т05)','request_for_calc_t05');">Сделать расчет</div>
						<div class="avt-button__fix avt-button__fix--white" onclick="callback_t05();">Консультация</div> -->
					</div>


				</div>	
</template>
<script>
export default {
	data(){
		return {
			warrenty: 'гарантия 25 лет',
			tickness: 'толщина 0,5 мм',
			zink: 'цинк 140 г/кв.м'

		}
	}
}
</script>

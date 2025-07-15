<script lang="ts">
	interface WorkExperience {
		jobTitle: string;
		company: string;
		startDate: string;
		endDate?: string;
	}
	const workExpeience: WorkExperience[] = [
		{ jobTitle: 'Bottle Washer', company: 'Vandelay Inc', startDate: '2002-03' },
		{ jobTitle: 'Asst. Nosač', company: 'Grad d.o.o.', startDate: '2002-03', endDate: '2018-08' },
		{ jobTitle: 'Bottle Washer I', company: 'Yadda', startDate: '2002-03', endDate: '2018-08' },
		{ jobTitle: 'Bottle Washer II', company: 'Yadda', startDate: '2002-03', endDate: '2018-08' }
	];
</script>

<section class="default-margin work-experience mt-m">
	<ul class="work-experience-list">
		{#each workExpeience as { jobTitle, company, startDate, endDate }}
			<li class="work-item">
				<article>
					<h3 class="semi-bold mb-xs">
						{jobTitle}
					</h3>
					<div class="company-and-date">
						<p>{company}</p>
						<p class="dark-gray">
							{startDate} {endDate ? ` / ${endDate}` : ` - present`}
						</p>
					</div>
				</article>
			</li>
		{/each}
	</ul>
	<h2 class="headline">
		Past work <br /> Experience
	</h2>
</section>

<style>
  .work-experience {
    display: flex;
    justify-content: space-between;
    width: 100%;
  }

  .work-experience-list {
    width: 50%;
  }

  .headline {
    text-align: right;
  }

  .work-item {
    border-bottom: 1px solid #f0eded;
  }

  .work-item:not(:first-of-type) {
    padding-top: 16px;
  }

  .work-item p {
    margin-bottom: 0;
  }

  .company-and-date {
    display: flex;
    justify-content: space-between;
  }
</style>
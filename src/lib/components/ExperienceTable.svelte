<script lang="ts">
  interface WorkExperience {
    jobTitle: string;
    company: string;
    startDate: string;
    endDate?: string;
  }
  const workExpeience: WorkExperience[] = [
    {jobTitle: 'Bottle Washer',
      company: 'Yadda',
      startDate: '2002-03'
    },
    {jobTitle: 'Bottle Washer',
      company: 'Yadda',
      startDate: '2002-03',
      endDate: '2018-08'
    },
    {jobTitle: 'Bottle Washer',
      company: 'Yadda',
      startDate: '2002-03',
      endDate: '2018-08'
    },
    {jobTitle: 'Bottle Washer',
      company: 'Yadda',
      startDate: '2002-03',
      endDate: '2018-08'
    },
  ]
</script>

<section class="default-margin work-experience mt-m">
	<ul class="work-experience-list">
    {#each workExpeience as {jobTitle, company}}
      <h3>{jobTitle} - {company}</h3>
    {/each}
  </ul>
	<h2 class="headline">
		Past work <br /> Experience
	</h2>
</section>
